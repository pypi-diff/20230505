# Comparing `tmp/robotframework-6.1a1.zip` & `tmp/robotframework-6.1b1.zip`

## zipinfo {}

```diff
@@ -1,302 +1,307 @@
-Zip file size: 704747 bytes, number of entries: 300
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/
--rw-rw-r--  2.0 unx    11358 b- defN 23-Jan-08 21:34 robotframework-6.1a1/LICENSE.txt
--rw-rw-r--  2.0 unx     6176 b- defN 23-Mar-10 21:51 robotframework-6.1a1/tasks.py
--rw-rw-r--  2.0 unx     9280 b- defN 23-Mar-14 09:13 robotframework-6.1a1/BUILD.rst
--rw-rw-r--  2.0 unx      607 b- defN 23-Jan-08 21:34 robotframework-6.1a1/COPYRIGHT.txt
--rw-rw-r--  2.0 unx    12212 b- defN 23-Mar-14 09:13 robotframework-6.1a1/INSTALL.rst
--rwxrwxr-x  2.0 unx     3359 b- defN 23-Mar-17 13:48 robotframework-6.1a1/setup.py
--rw-rw-r--  2.0 unx     5444 b- defN 23-Mar-14 09:13 robotframework-6.1a1/README.rst
--rw-rw-r--  2.0 unx    11985 b- defN 23-Mar-10 21:51 robotframework-6.1a1/CONTRIBUTING.rst
--rw-rw-r--  2.0 unx      228 b- defN 23-Jan-08 21:34 robotframework-6.1a1/MANIFEST.in
--rw-rw-r--  2.0 unx     6417 b- defN 23-Jan-08 21:34 robotframework-6.1a1/AUTHORS.rst
--rw-rw-r--  2.0 unx     8685 b- defN 23-Mar-17 13:48 robotframework-6.1a1/PKG-INFO
--rw-rw-r--  2.0 unx       38 b- defN 23-Mar-17 13:48 robotframework-6.1a1/setup.cfg
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robotframework.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/result/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/output/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/conf/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/variables/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/libdocpkg/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/reporting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/running/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/utils/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/htmldata/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/parsing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/libraries/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/api/
--rw-rw-r--  2.0 unx     1482 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/pythonpathsetter.py
--rwxrwxr-x  2.0 unx    22569 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/rebot.py
--rwxrwxr-x  2.0 unx    12653 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdoc.py
--rw-rw-r--  2.0 unx    10709 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/errors.py
--rwxrwxr-x  2.0 unx    11447 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/testdoc.py
--rw-rw-r--  2.0 unx     2121 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/__init__.py
--rw-rw-r--  2.0 unx     1405 b- defN 23-Mar-17 13:48 robotframework-6.1a1/src/robot/version.py
--rwxrwxr-x  2.0 unx      953 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/__main__.py
--rwxrwxr-x  2.0 unx    31743 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/run.py
--rw-rw-r--  2.0 unx    13220 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/result/xmlelementhandlers.py
--rw-rw-r--  2.0 unx     5760 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/result/executionresult.py
--rw-rw-r--  2.0 unx     1165 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/result/messagefilter.py
--rw-rw-r--  2.0 unx     2306 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/result/suiteteardownfailed.py
--rw-rw-r--  2.0 unx     2645 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/result/flattenkeywordmatcher.py
--rw-rw-r--  2.0 unx     5032 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/result/merger.py
--rw-rw-r--  2.0 unx     8276 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/result/resultbuilder.py
--rw-rw-r--  2.0 unx     1797 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/result/executionerrors.py
--rw-rw-r--  2.0 unx     1457 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/result/modeldeprecation.py
--rw-rw-r--  2.0 unx     2084 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/result/__init__.py
--rw-rw-r--  2.0 unx     5602 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/result/keywordremover.py
--rw-rw-r--  2.0 unx     3926 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/result/visitor.py
--rw-rw-r--  2.0 unx    25594 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/result/model.py
--rw-rw-r--  2.0 unx     2561 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/result/configurer.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/output/console/
--rw-rw-r--  2.0 unx     6772 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/output/listeners.py
--rw-rw-r--  2.0 unx     3368 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/output/output.py
--rw-rw-r--  2.0 unx     3797 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/output/listenermethods.py
--rw-rw-r--  2.0 unx     2678 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/output/pyloggingconf.py
--rw-rw-r--  2.0 unx     1899 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/output/filelogger.py
--rw-rw-r--  2.0 unx     5159 b- defN 23-Mar-14 10:12 robotframework-6.1a1/src/robot/output/loggerhelper.py
--rw-rw-r--  2.0 unx     2257 b- defN 23-Mar-14 11:08 robotframework-6.1a1/src/robot/output/stdoutlogsplitter.py
--rw-rw-r--  2.0 unx    10129 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/output/logger.py
--rw-rw-r--  2.0 unx     2098 b- defN 23-Mar-14 10:12 robotframework-6.1a1/src/robot/output/librarylogger.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/output/__init__.py
--rw-rw-r--  2.0 unx     3507 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/output/debugfile.py
--rw-rw-r--  2.0 unx    10513 b- defN 23-Mar-15 01:54 robotframework-6.1a1/src/robot/output/xmllogger.py
--rw-rw-r--  2.0 unx     6040 b- defN 23-Mar-15 11:19 robotframework-6.1a1/src/robot/output/listenerarguments.py
--rw-rw-r--  2.0 unx     1005 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/output/console/quiet.py
--rw-rw-r--  2.0 unx     6034 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/output/console/verbose.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/output/console/__init__.py
--rw-rw-r--  2.0 unx     3434 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/output/console/dotted.py
--rw-rw-r--  2.0 unx     6807 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/output/console/highlighting.py
--rw-rw-r--  2.0 unx     2457 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/message.py
--rw-rw-r--  2.0 unx     5599 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/stats.py
--rw-rw-r--  2.0 unx     6439 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/testcase.py
--rw-rw-r--  2.0 unx     5432 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/model/tags.py
--rw-rw-r--  2.0 unx     1271 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/fixture.py
--rw-rw-r--  2.0 unx     8723 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/body.py
--rw-rw-r--  2.0 unx     6604 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/itemlist.py
--rw-rw-r--  2.0 unx    11359 b- defN 23-Mar-16 14:42 robotframework-6.1a1/src/robot/model/testsuite.py
--rw-rw-r--  2.0 unx    10832 b- defN 23-Mar-17 01:21 robotframework-6.1a1/src/robot/model/control.py
--rw-rw-r--  2.0 unx     1112 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/model/metadata.py
--rw-rw-r--  2.0 unx     2218 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/suitestatistics.py
--rw-rw-r--  2.0 unx     2115 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/model/modifier.py
--rw-rw-r--  2.0 unx     4302 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/keyword.py
--rw-rw-r--  2.0 unx     1528 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/namepatterns.py
--rw-rw-r--  2.0 unx     1097 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/tagsetter.py
--rw-rw-r--  2.0 unx     1829 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/__init__.py
--rw-rw-r--  2.0 unx    21084 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/model/visitor.py
--rw-rw-r--  2.0 unx     2615 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/totalstatistics.py
--rw-rw-r--  2.0 unx     3841 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/model/filter.py
--rw-rw-r--  2.0 unx     7512 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/model/modelobject.py
--rw-rw-r--  2.0 unx     3400 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/model/configurer.py
--rw-rw-r--  2.0 unx     2632 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/statistics.py
--rw-rw-r--  2.0 unx     4992 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/model/tagstatistics.py
--rw-rw-r--  2.0 unx    26134 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/conf/settings.py
--rw-rw-r--  2.0 unx     1226 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/conf/__init__.py
--rw-rw-r--  2.0 unx    46409 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/conf/languages.py
--rw-rw-r--  2.0 unx     2555 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/conf/gatherfailed.py
--rw-rw-r--  2.0 unx     2823 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/variables.py
--rw-rw-r--  2.0 unx     9222 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/scopes.py
--rw-rw-r--  2.0 unx     4421 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/variables/store.py
--rw-rw-r--  2.0 unx     8199 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/variables/search.py
--rw-rw-r--  2.0 unx     8968 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/replacer.py
--rw-rw-r--  2.0 unx     8602 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/assigner.py
--rw-rw-r--  2.0 unx     1729 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/variables/notfound.py
--rw-rw-r--  2.0 unx     4747 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/finders.py
--rw-rw-r--  2.0 unx     1380 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/variables/__init__.py
--rw-rw-r--  2.0 unx     6798 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/filesetter.py
--rw-rw-r--  2.0 unx     5683 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/variables/evaluation.py
--rw-rw-r--  2.0 unx     5348 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/variables/tablesetter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/variables/resolvable.py
--rw-rw-r--  2.0 unx     1172 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libdocpkg/writer.py
--rw-rw-r--  2.0 unx     4620 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/builder.py
--rw-rw-r--  2.0 unx     5673 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/jsonbuilder.py
--rw-rw-r--  2.0 unx     1397 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libdocpkg/htmlwriter.py
--rw-rw-r--  2.0 unx     1767 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libdocpkg/output.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/libdocpkg/jsonwriter.py
--rw-rw-r--  2.0 unx     6943 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/xmlwriter.py
--rw-rw-r--  2.0 unx     7609 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/standardtypes.py
--rw-rw-r--  2.0 unx     7130 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/robotbuilder.py
--rwxrwxr-x  2.0 unx     3586 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/libdocpkg/consoleviewer.py
--rw-rw-r--  2.0 unx     4311 b- defN 23-Mar-10 21:54 robotframework-6.1a1/src/robot/libdocpkg/datatypes.py
--rw-rw-r--  2.0 unx      835 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/__init__.py
--rw-rw-r--  2.0 unx     5293 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libdocpkg/htmlutils.py
--rw-rw-r--  2.0 unx     7993 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/model.py
--rw-rw-r--  2.0 unx     7082 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libdocpkg/xmlbuilder.py
--rw-rw-r--  2.0 unx     3409 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/reporting/xunitwriter.py
--rw-rw-r--  2.0 unx     8029 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/reporting/jsmodelbuilders.py
--rw-rw-r--  2.0 unx     3984 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/reporting/jsbuildingcontext.py
--rw-rw-r--  2.0 unx     4022 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/reporting/jswriter.py
--rw-rw-r--  2.0 unx     1671 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/reporting/stringcache.py
--rw-rw-r--  2.0 unx     1192 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/reporting/__init__.py
--rw-rw-r--  2.0 unx     5674 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/reporting/resultwriter.py
--rw-rw-r--  2.0 unx     2482 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/reporting/logreportwriters.py
--rw-rw-r--  2.0 unx     3525 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/reporting/jsexecutionresult.py
--rw-rw-r--  2.0 unx     1044 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/reporting/outputwriter.py
--rw-rw-r--  2.0 unx     1412 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/reporting/expandkeywordmatcher.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/running/timeouts/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/running/builder/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/running/arguments/
--rw-rw-r--  2.0 unx     7411 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/context.py
--rw-rw-r--  2.0 unx     9415 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/librarykeywordrunner.py
--rw-rw-r--  2.0 unx    11770 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/handlers.py
--rw-rw-r--  2.0 unx     1159 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/modelcombiner.py
--rw-rw-r--  2.0 unx     2602 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/libraryscopes.py
--rw-rw-r--  2.0 unx     3072 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/signalhandler.py
--rw-rw-r--  2.0 unx    10918 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/running/userkeywordrunner.py
--rw-rw-r--  2.0 unx    26698 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/bodyrunner.py
--rw-rw-r--  2.0 unx     2647 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/running/usererrorhandler.py
--rw-rw-r--  2.0 unx    10975 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/running/suiterunner.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Mar-15 16:57 robotframework-6.1a1/src/robot/running/status.py
--rw-rw-r--  2.0 unx     3720 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/runkwregister.py
--rw-rw-r--  2.0 unx    15721 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/testlibraries.py
--rw-rw-r--  2.0 unx     3334 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/outputcapture.py
--rw-rw-r--  2.0 unx     3966 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/running/userkeyword.py
--rw-rw-r--  2.0 unx     4529 b- defN 23-Mar-17 01:17 robotframework-6.1a1/src/robot/running/__init__.py
--rw-rw-r--  2.0 unx     1772 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/randomizer.py
--rw-rw-r--  2.0 unx    22162 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/namespace.py
--rw-rw-r--  2.0 unx     3428 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/statusreporter.py
--rw-rw-r--  2.0 unx     2366 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/handlerstore.py
--rw-rw-r--  2.0 unx     4787 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/dynamicmethods.py
--rw-rw-r--  2.0 unx    28253 b- defN 23-Mar-17 01:19 robotframework-6.1a1/src/robot/running/model.py
--rw-rw-r--  2.0 unx     5816 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/importer.py
--rw-rw-r--  2.0 unx     1240 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/timeouts/posix.py
--rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/timeouts/__init__.py
--rw-rw-r--  2.0 unx     2320 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/timeouts/windows.py
--rw-rw-r--  2.0 unx     3684 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/builder/parsers.py
--rw-rw-r--  2.0 unx    22149 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/running/builder/transformers.py
--rw-rw-r--  2.0 unx     3432 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/builder/settings.py
--rw-rw-r--  2.0 unx     9268 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/builder/builders.py
--rw-rw-r--  2.0 unx      737 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/running/builder/__init__.py
--rw-rw-r--  2.0 unx     2975 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/arguments/argumentmapper.py
--rw-rw-r--  2.0 unx     3475 b- defN 23-Mar-10 21:54 robotframework-6.1a1/src/robot/running/arguments/argumentconverter.py
--rw-rw-r--  2.0 unx     4980 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/arguments/argumentresolver.py
--rw-rw-r--  2.0 unx     5939 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/arguments/embedded.py
--rw-rw-r--  2.0 unx     4191 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/arguments/customconverters.py
--rw-rw-r--  2.0 unx    25528 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/arguments/typeconverters.py
--rw-rw-r--  2.0 unx     2331 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/running/arguments/typevalidator.py
--rw-rw-r--  2.0 unx     8547 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/arguments/argumentspec.py
--rw-rw-r--  2.0 unx     7703 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/arguments/argumentparser.py
--rw-rw-r--  2.0 unx     4349 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/running/arguments/argumentvalidator.py
--rw-rw-r--  2.0 unx     1010 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/running/arguments/__init__.py
--rw-rw-r--  2.0 unx     2052 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/robotio.py
--rw-rw-r--  2.0 unx     3314 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/filereader.py
--rw-rw-r--  2.0 unx     1586 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/sortable.py
--rw-rw-r--  2.0 unx     4102 b- defN 23-Mar-15 02:28 robotframework-6.1a1/src/robot/utils/escaping.py
--rw-rw-r--  2.0 unx     2956 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/restreader.py
--rw-rw-r--  2.0 unx     1955 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/frange.py
--rw-rw-r--  2.0 unx     6131 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/connectioncache.py
--rw-rw-r--  2.0 unx     3842 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/normalizing.py
--rw-rw-r--  2.0 unx     3956 b- defN 23-Mar-15 01:46 robotframework-6.1a1/src/robot/utils/markupwriters.py
--rw-rw-r--  2.0 unx     1587 b- defN 23-Mar-16 14:42 robotframework-6.1a1/src/robot/utils/setter.py
--rw-rw-r--  2.0 unx      809 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/compress.py
--rw-rw-r--  2.0 unx     5373 b- defN 23-Mar-15 02:28 robotframework-6.1a1/src/robot/utils/misc.py
--rw-rw-r--  2.0 unx     2254 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/dotdict.py
--rw-rw-r--  2.0 unx     3721 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/recommendations.py
--rw-rw-r--  2.0 unx     5355 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/text.py
--rw-rw-r--  2.0 unx     2149 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/unic.py
--rw-rw-r--  2.0 unx     1664 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/markuputils.py
--rw-rw-r--  2.0 unx     5391 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/utils/robotpath.py
--rw-rw-r--  2.0 unx    16133 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/utils/robottime.py
--rw-rw-r--  2.0 unx     3148 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/encoding.py
--rw-rw-r--  2.0 unx     3262 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/encodingsniffer.py
--rw-rw-r--  2.0 unx    15859 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/utils/argumentparser.py
--rw-rw-r--  2.0 unx     8776 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/asserts.py
--rw-rw-r--  2.0 unx     4561 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/utils/__init__.py
--rw-rw-r--  2.0 unx     4300 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/application.py
--rw-rw-r--  2.0 unx     2635 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/etreewrapper.py
--rw-rw-r--  2.0 unx     2701 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/match.py
--rw-rw-r--  2.0 unx     4673 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/error.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/utils/robotenv.py
--rw-rw-r--  2.0 unx     9851 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/htmlformatters.py
--rw-rw-r--  2.0 unx     7487 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/charwidth.py
--rw-rw-r--  2.0 unx     1389 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/platform.py
--rw-rw-r--  2.0 unx    13504 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/utils/importer.py
--rw-rw-r--  2.0 unx      902 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/utils/robotinspect.py
--rw-rw-r--  2.0 unx     5565 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/utils/robottypes.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/htmldata/libdoc/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/htmldata/rebot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/htmldata/lib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/htmldata/testdoc/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/htmldata/common/
--rw-rw-r--  2.0 unx     4127 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/htmldata/jsonwriter.py
--rw-rw-r--  2.0 unx     3457 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/htmldata/htmlfilewriter.py
--rw-rw-r--  2.0 unx     1062 b- defN 23-Mar-14 13:09 robotframework-6.1a1/src/robot/htmldata/template.py
--rw-rw-r--  2.0 unx      981 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/__init__.py
--rw-rw-r--  2.0 unx      138 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/libdoc/print.css
--rw-rw-r--  2.0 unx    14346 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/htmldata/libdoc/libdoc.css
--rw-rw-r--  2.0 unx    28636 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/htmldata/libdoc/libdoc.html
--rw-rw-r--  2.0 unx     8894 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/libdoc/pygments.css
--rw-rw-r--  2.0 unx     1341 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/libdoc/doc_formatting.css
--rw-rw-r--  2.0 unx     4646 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/common.css
--rw-rw-r--  2.0 unx     3413 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/report.css
--rw-rw-r--  2.0 unx     6955 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/htmldata/rebot/log.js
--rw-rw-r--  2.0 unx      699 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/print.css
--rw-rw-r--  2.0 unx     6510 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/view.js
--rw-rw-r--  2.0 unx    30836 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/report.html
--rw-rw-r--  2.0 unx    10023 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/htmldata/rebot/testdata.js
--rw-rw-r--  2.0 unx     7155 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/util.js
--rw-rw-r--  2.0 unx    11525 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/htmldata/rebot/model.js
--rw-rw-r--  2.0 unx    15416 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/htmldata/rebot/log.html
--rw-rw-r--  2.0 unx     1487 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/fileloading.js
--rw-rw-r--  2.0 unx      903 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/rebot/doc_formatting.css
--rw-rw-r--  2.0 unx     7390 b- defN 23-Feb-28 18:30 robotframework-6.1a1/src/robot/htmldata/rebot/log.css
--rw-rw-r--  2.0 unx    13667 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/lib/jsxcompressor.min.js
--rw-rw-r--  2.0 unx    43881 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/lib/jquery.tablesorter.min.js
--rw-rw-r--  2.0 unx     1524 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/lib/jquery.highlight.min.js
--rw-rw-r--  2.0 unx    89476 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/lib/jquery.min.js
--rw-rw-r--  2.0 unx     6141 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/lib/jquery.tmpl.min.js
--rw-rw-r--  2.0 unx      153 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/testdoc/testdoc.css
--rw-rw-r--  2.0 unx     9765 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/testdoc/testdoc.html
--rw-rw-r--  2.0 unx      872 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/common/storage.js
--rw-rw-r--  2.0 unx      373 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/htmldata/common/js_disabled.css
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/parsing/model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/parsing/parser/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-17 13:48 robotframework-6.1a1/src/robot/parsing/lexer/
--rw-rw-r--  2.0 unx     6073 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/parsing/suitestructure.py
--rw-rw-r--  2.0 unx     1237 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/parsing/__init__.py
--rw-rw-r--  2.0 unx    12939 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/model/blocks.py
--rw-rw-r--  2.0 unx      937 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/model/__init__.py
--rw-rw-r--  2.0 unx     2301 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/parsing/model/visitor.py
--rw-rw-r--  2.0 unx    35669 b- defN 23-Mar-16 23:30 robotframework-6.1a1/src/robot/parsing/model/statements.py
--rw-rw-r--  2.0 unx     3902 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/parser/blockparsers.py
--rw-rw-r--  2.0 unx     4581 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/parsing/parser/parser.py
--rw-rw-r--  2.0 unx      710 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/parsing/parser/__init__.py
--rw-rw-r--  2.0 unx     3678 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/parser/fileparser.py
--rw-rw-r--  2.0 unx     7044 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/parsing/lexer/lexer.py
--rw-rw-r--  2.0 unx    10996 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/lexer/blocklexers.py
--rw-rw-r--  2.0 unx     4744 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/lexer/context.py
--rw-rw-r--  2.0 unx     7569 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/parsing/lexer/settings.py
--rw-rw-r--  2.0 unx     8871 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/lexer/tokens.py
--rw-rw-r--  2.0 unx    10119 b- defN 23-Mar-16 21:20 robotframework-6.1a1/src/robot/parsing/lexer/statementlexers.py
--rw-rw-r--  2.0 unx      738 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/parsing/lexer/__init__.py
--rw-rw-r--  2.0 unx     5145 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/parsing/lexer/tokenizer.py
--rw-rw-r--  2.0 unx    71518 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/XML.py
--rw-rw-r--  2.0 unx    14289 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Screenshot.py
--rw-rw-r--  2.0 unx     1104 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/libraries/Easter.py
--rw-rw-r--  2.0 unx     5960 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/libraries/dialogs_py.py
--rw-rw-r--  2.0 unx    36128 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/String.py
--rw-rw-r--  2.0 unx    54972 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Telnet.py
--rw-rw-r--  2.0 unx    28349 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/DateTime.py
--rw-rw-r--  2.0 unx    10309 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Remote.py
--rw-rw-r--  2.0 unx    64676 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/OperatingSystem.py
--rw-rw-r--  2.0 unx    43712 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Collections.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/libraries/__init__.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Reserved.py
--rw-rw-r--  2.0 unx     4567 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Dialogs.py
--rw-rw-r--  2.0 unx   187410 b- defN 23-Mar-14 11:30 robotframework-6.1a1/src/robot/libraries/BuiltIn.py
--rw-rw-r--  2.0 unx    45060 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/libraries/Process.py
--rw-rw-r--  2.0 unx    19771 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/api/interfaces.py
--rw-rw-r--  2.0 unx    21142 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/api/parsing.py
--rw-rw-r--  2.0 unx     5157 b- defN 23-Mar-10 21:51 robotframework-6.1a1/src/robot/api/deco.py
--rw-rw-r--  2.0 unx     4918 b- defN 23-Mar-14 10:43 robotframework-6.1a1/src/robot/api/logger.py
--rw-rw-r--  2.0 unx     4001 b- defN 23-Mar-14 09:13 robotframework-6.1a1/src/robot/api/__init__.py
--rw-rw-r--  2.0 unx     3140 b- defN 23-Jan-08 21:34 robotframework-6.1a1/src/robot/api/exceptions.py
--rw-rw-r--  2.0 unx     8743 b- defN 23-Mar-17 13:48 robotframework-6.1a1/src/robotframework.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      108 b- defN 23-Mar-17 13:48 robotframework-6.1a1/src/robotframework.egg-info/entry_points.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-17 13:48 robotframework-6.1a1/src/robotframework.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     8685 b- defN 23-Mar-17 13:48 robotframework-6.1a1/src/robotframework.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 23-Mar-17 13:48 robotframework-6.1a1/src/robotframework.egg-info/top_level.txt
-300 files, 2286592 bytes uncompressed, 651185 bytes compressed:  71.5%
+Zip file size: 719096 bytes, number of entries: 305
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/
+-rw-rw-r--  2.0 unx    11358 b- defN 23-Jan-08 21:34 robotframework-6.1b1/LICENSE.txt
+-rw-rw-r--  2.0 unx     6176 b- defN 23-Mar-10 21:51 robotframework-6.1b1/tasks.py
+-rw-rw-r--  2.0 unx     9280 b- defN 23-Mar-28 14:56 robotframework-6.1b1/BUILD.rst
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jan-08 21:34 robotframework-6.1b1/COPYRIGHT.txt
+-rw-rw-r--  2.0 unx    12212 b- defN 23-Mar-28 14:56 robotframework-6.1b1/INSTALL.rst
+-rwxrwxr-x  2.0 unx     3359 b- defN 23-May-05 21:12 robotframework-6.1b1/setup.py
+-rw-rw-r--  2.0 unx     5444 b- defN 23-Mar-28 14:56 robotframework-6.1b1/README.rst
+-rw-rw-r--  2.0 unx    11985 b- defN 23-Mar-10 21:51 robotframework-6.1b1/CONTRIBUTING.rst
+-rw-rw-r--  2.0 unx      228 b- defN 23-Jan-08 21:34 robotframework-6.1b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     6417 b- defN 23-Jan-08 21:34 robotframework-6.1b1/AUTHORS.rst
+-rw-rw-r--  2.0 unx     8685 b- defN 23-May-05 21:54 robotframework-6.1b1/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-05 21:54 robotframework-6.1b1/setup.cfg
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/result/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/output/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/conf/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/variables/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/libdocpkg/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/reporting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/utils/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/libraries/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/api/
+-rw-rw-r--  2.0 unx     1353 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/pythonpathsetter.py
+-rwxrwxr-x  2.0 unx    22432 b- defN 23-Apr-12 21:16 robotframework-6.1b1/src/robot/rebot.py
+-rwxrwxr-x  2.0 unx    12523 b- defN 23-Apr-12 21:16 robotframework-6.1b1/src/robot/libdoc.py
+-rw-rw-r--  2.0 unx    10709 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/errors.py
+-rwxrwxr-x  2.0 unx    11316 b- defN 23-Apr-12 21:16 robotframework-6.1b1/src/robot/testdoc.py
+-rw-rw-r--  2.0 unx     2121 b- defN 23-Mar-30 02:33 robotframework-6.1b1/src/robot/__init__.py
+-rw-rw-r--  2.0 unx     1405 b- defN 23-May-05 21:12 robotframework-6.1b1/src/robot/version.py
+-rwxrwxr-x  2.0 unx      803 b- defN 23-Apr-12 21:14 robotframework-6.1b1/src/robot/__main__.py
+-rwxrwxr-x  2.0 unx    31972 b- defN 23-Apr-26 10:51 robotframework-6.1b1/src/robot/run.py
+-rw-rw-r--  2.0 unx    13316 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/result/xmlelementhandlers.py
+-rw-rw-r--  2.0 unx     5760 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/executionresult.py
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/messagefilter.py
+-rw-rw-r--  2.0 unx     2306 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/suiteteardownfailed.py
+-rw-rw-r--  2.0 unx     2645 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/result/flattenkeywordmatcher.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/result/merger.py
+-rw-rw-r--  2.0 unx     8276 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/result/resultbuilder.py
+-rw-rw-r--  2.0 unx     1797 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/result/executionerrors.py
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/modeldeprecation.py
+-rw-rw-r--  2.0 unx     2084 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/result/__init__.py
+-rw-rw-r--  2.0 unx     5614 b- defN 23-Apr-04 23:22 robotframework-6.1b1/src/robot/result/keywordremover.py
+-rw-rw-r--  2.0 unx     3926 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/result/visitor.py
+-rw-rw-r--  2.0 unx    25861 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/result/model.py
+-rw-rw-r--  2.0 unx     2561 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/result/configurer.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/output/console/
+-rw-rw-r--  2.0 unx     6772 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/listeners.py
+-rw-rw-r--  2.0 unx     3368 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/output/output.py
+-rw-rw-r--  2.0 unx     3797 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/listenermethods.py
+-rw-rw-r--  2.0 unx     2678 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/pyloggingconf.py
+-rw-rw-r--  2.0 unx     1899 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/filelogger.py
+-rw-rw-r--  2.0 unx     5159 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/loggerhelper.py
+-rw-rw-r--  2.0 unx     2257 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/stdoutlogsplitter.py
+-rw-rw-r--  2.0 unx    10129 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/output/logger.py
+-rw-rw-r--  2.0 unx     2098 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/librarylogger.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/output/__init__.py
+-rw-rw-r--  2.0 unx     3507 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/output/debugfile.py
+-rw-rw-r--  2.0 unx    10611 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/output/xmllogger.py
+-rw-rw-r--  2.0 unx     6060 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/listenerarguments.py
+-rw-rw-r--  2.0 unx     1005 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/console/quiet.py
+-rw-rw-r--  2.0 unx     6034 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/console/verbose.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/output/console/__init__.py
+-rw-rw-r--  2.0 unx     3434 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/console/dotted.py
+-rw-rw-r--  2.0 unx     6807 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/console/highlighting.py
+-rw-rw-r--  2.0 unx     2540 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/model/message.py
+-rw-rw-r--  2.0 unx     5611 b- defN 23-Apr-04 23:06 robotframework-6.1b1/src/robot/model/stats.py
+-rw-rw-r--  2.0 unx     7197 b- defN 23-Apr-06 17:11 robotframework-6.1b1/src/robot/model/testcase.py
+-rw-rw-r--  2.0 unx     6968 b- defN 23-Apr-25 18:26 robotframework-6.1b1/src/robot/model/tags.py
+-rw-rw-r--  2.0 unx     1312 b- defN 23-Apr-04 23:37 robotframework-6.1b1/src/robot/model/fixture.py
+-rw-rw-r--  2.0 unx     8818 b- defN 23-Apr-06 20:10 robotframework-6.1b1/src/robot/model/body.py
+-rw-rw-r--  2.0 unx     7742 b- defN 23-Apr-05 17:01 robotframework-6.1b1/src/robot/model/itemlist.py
+-rw-rw-r--  2.0 unx    12228 b- defN 23-Apr-28 16:14 robotframework-6.1b1/src/robot/model/testsuite.py
+-rw-rw-r--  2.0 unx    11299 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/model/control.py
+-rw-rw-r--  2.0 unx     1112 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/model/metadata.py
+-rw-rw-r--  2.0 unx     2218 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/suitestatistics.py
+-rw-rw-r--  2.0 unx     2115 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/model/modifier.py
+-rw-rw-r--  2.0 unx     4933 b- defN 23-Apr-06 17:11 robotframework-6.1b1/src/robot/model/keyword.py
+-rw-rw-r--  2.0 unx     1682 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/model/namepatterns.py
+-rw-rw-r--  2.0 unx     1360 b- defN 23-Apr-04 19:08 robotframework-6.1b1/src/robot/model/tagsetter.py
+-rw-rw-r--  2.0 unx     1829 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/model/__init__.py
+-rw-rw-r--  2.0 unx    21366 b- defN 23-May-05 21:05 robotframework-6.1b1/src/robot/model/visitor.py
+-rw-rw-r--  2.0 unx     2615 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/totalstatistics.py
+-rw-rw-r--  2.0 unx     4060 b- defN 23-Apr-05 00:37 robotframework-6.1b1/src/robot/model/filter.py
+-rw-rw-r--  2.0 unx     7512 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/model/modelobject.py
+-rw-rw-r--  2.0 unx     3400 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/model/configurer.py
+-rw-rw-r--  2.0 unx     2632 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/statistics.py
+-rw-rw-r--  2.0 unx     4992 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/tagstatistics.py
+-rw-rw-r--  2.0 unx    26226 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/conf/settings.py
+-rw-rw-r--  2.0 unx     1255 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/conf/__init__.py
+-rw-rw-r--  2.0 unx    47767 b- defN 23-May-03 17:44 robotframework-6.1b1/src/robot/conf/languages.py
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/conf/gatherfailed.py
+-rw-rw-r--  2.0 unx     2823 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/variables.py
+-rw-rw-r--  2.0 unx     9222 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/variables/scopes.py
+-rw-rw-r--  2.0 unx     4421 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/store.py
+-rw-rw-r--  2.0 unx     8339 b- defN 23-Apr-05 21:52 robotframework-6.1b1/src/robot/variables/search.py
+-rw-rw-r--  2.0 unx     8968 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/replacer.py
+-rw-rw-r--  2.0 unx     8602 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/assigner.py
+-rw-rw-r--  2.0 unx     1729 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/variables/notfound.py
+-rw-rw-r--  2.0 unx     4747 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/finders.py
+-rw-rw-r--  2.0 unx     1380 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/__init__.py
+-rw-rw-r--  2.0 unx     6798 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/variables/filesetter.py
+-rw-rw-r--  2.0 unx     5683 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/evaluation.py
+-rw-rw-r--  2.0 unx     5348 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/tablesetter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/resolvable.py
+-rw-rw-r--  2.0 unx     1172 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/writer.py
+-rw-rw-r--  2.0 unx     4620 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/builder.py
+-rw-rw-r--  2.0 unx     5673 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/libdocpkg/jsonbuilder.py
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/htmlwriter.py
+-rw-rw-r--  2.0 unx     1767 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/output.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/libdocpkg/jsonwriter.py
+-rw-rw-r--  2.0 unx     6943 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/xmlwriter.py
+-rw-rw-r--  2.0 unx     7609 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/standardtypes.py
+-rw-rw-r--  2.0 unx     7130 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/libdocpkg/robotbuilder.py
+-rwxrwxr-x  2.0 unx     3586 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/libdocpkg/consoleviewer.py
+-rw-rw-r--  2.0 unx     4311 b- defN 23-Mar-10 21:54 robotframework-6.1b1/src/robot/libdocpkg/datatypes.py
+-rw-rw-r--  2.0 unx      835 b- defN 23-Mar-14 09:13 robotframework-6.1b1/src/robot/libdocpkg/__init__.py
+-rw-rw-r--  2.0 unx     5293 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/htmlutils.py
+-rw-rw-r--  2.0 unx     7993 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/model.py
+-rw-rw-r--  2.0 unx     7082 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/libdocpkg/xmlbuilder.py
+-rw-rw-r--  2.0 unx     3409 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/reporting/xunitwriter.py
+-rw-rw-r--  2.0 unx     8029 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/reporting/jsmodelbuilders.py
+-rw-rw-r--  2.0 unx     3984 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/reporting/jsbuildingcontext.py
+-rw-rw-r--  2.0 unx     4022 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/reporting/jswriter.py
+-rw-rw-r--  2.0 unx     1671 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/reporting/stringcache.py
+-rw-rw-r--  2.0 unx     1192 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/reporting/__init__.py
+-rw-rw-r--  2.0 unx     5674 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/reporting/resultwriter.py
+-rw-rw-r--  2.0 unx     2482 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/reporting/logreportwriters.py
+-rw-rw-r--  2.0 unx     3525 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/reporting/jsexecutionresult.py
+-rw-rw-r--  2.0 unx     1044 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/reporting/outputwriter.py
+-rw-rw-r--  2.0 unx     1498 b- defN 23-May-04 19:41 robotframework-6.1b1/src/robot/reporting/expandkeywordmatcher.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/timeouts/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/builder/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/arguments/
+-rw-rw-r--  2.0 unx     8505 b- defN 23-Apr-05 21:52 robotframework-6.1b1/src/robot/running/context.py
+-rw-rw-r--  2.0 unx     9604 b- defN 23-Apr-05 17:43 robotframework-6.1b1/src/robot/running/librarykeywordrunner.py
+-rw-rw-r--  2.0 unx    11770 b- defN 23-Apr-24 20:14 robotframework-6.1b1/src/robot/running/handlers.py
+-rw-rw-r--  2.0 unx     1159 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/modelcombiner.py
+-rw-rw-r--  2.0 unx     2602 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/libraryscopes.py
+-rw-rw-r--  2.0 unx     3072 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/signalhandler.py
+-rw-rw-r--  2.0 unx    10918 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/userkeywordrunner.py
+-rw-rw-r--  2.0 unx    28966 b- defN 23-May-05 16:04 robotframework-6.1b1/src/robot/running/bodyrunner.py
+-rw-rw-r--  2.0 unx     2647 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/usererrorhandler.py
+-rw-rw-r--  2.0 unx    11206 b- defN 23-Apr-25 17:25 robotframework-6.1b1/src/robot/running/suiterunner.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Mar-15 16:57 robotframework-6.1b1/src/robot/running/status.py
+-rw-rw-r--  2.0 unx     3720 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/runkwregister.py
+-rw-rw-r--  2.0 unx    15721 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/testlibraries.py
+-rw-rw-r--  2.0 unx     3334 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/outputcapture.py
+-rw-rw-r--  2.0 unx     3966 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/userkeyword.py
+-rw-rw-r--  2.0 unx     4803 b- defN 23-May-05 20:41 robotframework-6.1b1/src/robot/running/__init__.py
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/randomizer.py
+-rw-rw-r--  2.0 unx    22162 b- defN 23-Apr-24 20:15 robotframework-6.1b1/src/robot/running/namespace.py
+-rw-rw-r--  2.0 unx     3399 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/statusreporter.py
+-rw-rw-r--  2.0 unx     2366 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/handlerstore.py
+-rw-rw-r--  2.0 unx     4787 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/dynamicmethods.py
+-rw-rw-r--  2.0 unx    29220 b- defN 23-May-02 15:52 robotframework-6.1b1/src/robot/running/model.py
+-rw-rw-r--  2.0 unx     5816 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/importer.py
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/timeouts/posix.py
+-rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/timeouts/__init__.py
+-rw-rw-r--  2.0 unx     2320 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/timeouts/windows.py
+-rw-rw-r--  2.0 unx     6444 b- defN 23-Apr-28 15:47 robotframework-6.1b1/src/robot/running/builder/parsers.py
+-rw-rw-r--  2.0 unx    22451 b- defN 23-May-03 02:14 robotframework-6.1b1/src/robot/running/builder/transformers.py
+-rw-rw-r--  2.0 unx     6737 b- defN 23-May-05 20:30 robotframework-6.1b1/src/robot/running/builder/settings.py
+-rw-rw-r--  2.0 unx    12795 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/running/builder/builders.py
+-rw-rw-r--  2.0 unx      772 b- defN 23-Apr-25 21:50 robotframework-6.1b1/src/robot/running/builder/__init__.py
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/arguments/argumentmapper.py
+-rw-rw-r--  2.0 unx     3475 b- defN 23-Mar-10 21:54 robotframework-6.1b1/src/robot/running/arguments/argumentconverter.py
+-rw-rw-r--  2.0 unx     4980 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/arguments/argumentresolver.py
+-rw-rw-r--  2.0 unx     5939 b- defN 23-Mar-14 09:13 robotframework-6.1b1/src/robot/running/arguments/embedded.py
+-rw-rw-r--  2.0 unx     4291 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/running/arguments/customconverters.py
+-rw-rw-r--  2.0 unx    26053 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/arguments/typeconverters.py
+-rw-rw-r--  2.0 unx     2331 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/arguments/typevalidator.py
+-rw-rw-r--  2.0 unx     8547 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/arguments/argumentspec.py
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/running/arguments/argumentparser.py
+-rw-rw-r--  2.0 unx     4349 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/running/arguments/argumentvalidator.py
+-rw-rw-r--  2.0 unx     1010 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/arguments/__init__.py
+-rw-rw-r--  2.0 unx     2052 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/robotio.py
+-rw-rw-r--  2.0 unx     3542 b- defN 23-Apr-21 15:51 robotframework-6.1b1/src/robot/utils/filereader.py
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/sortable.py
+-rw-rw-r--  2.0 unx     4102 b- defN 23-Mar-15 02:28 robotframework-6.1b1/src/robot/utils/escaping.py
+-rw-rw-r--  2.0 unx     2956 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/restreader.py
+-rw-rw-r--  2.0 unx     1955 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/frange.py
+-rw-rw-r--  2.0 unx     6131 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/connectioncache.py
+-rw-rw-r--  2.0 unx     4314 b- defN 23-Apr-28 17:01 robotframework-6.1b1/src/robot/utils/normalizing.py
+-rw-rw-r--  2.0 unx     3956 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/utils/markupwriters.py
+-rw-rw-r--  2.0 unx     3202 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/utils/setter.py
+-rw-rw-r--  2.0 unx      809 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/compress.py
+-rw-rw-r--  2.0 unx     5373 b- defN 23-Apr-28 17:15 robotframework-6.1b1/src/robot/utils/misc.py
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/dotdict.py
+-rw-rw-r--  2.0 unx     3721 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/recommendations.py
+-rw-rw-r--  2.0 unx     5436 b- defN 23-Apr-27 02:29 robotframework-6.1b1/src/robot/utils/text.py
+-rw-rw-r--  2.0 unx     2149 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/unic.py
+-rw-rw-r--  2.0 unx     1664 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/markuputils.py
+-rw-rw-r--  2.0 unx     5391 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/utils/robotpath.py
+-rw-rw-r--  2.0 unx    16133 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/utils/robottime.py
+-rw-rw-r--  2.0 unx     3221 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/utils/encoding.py
+-rw-rw-r--  2.0 unx     3262 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/encodingsniffer.py
+-rw-rw-r--  2.0 unx    15942 b- defN 23-Apr-24 23:28 robotframework-6.1b1/src/robot/utils/argumentparser.py
+-rw-rw-r--  2.0 unx     8776 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/asserts.py
+-rw-rw-r--  2.0 unx     4569 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/utils/__init__.py
+-rw-rw-r--  2.0 unx     4300 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/application.py
+-rw-rw-r--  2.0 unx     2635 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/etreewrapper.py
+-rw-rw-r--  2.0 unx     3042 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/utils/match.py
+-rw-rw-r--  2.0 unx     4673 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/error.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/utils/robotenv.py
+-rw-rw-r--  2.0 unx     9851 b- defN 23-Mar-27 20:53 robotframework-6.1b1/src/robot/utils/htmlformatters.py
+-rw-rw-r--  2.0 unx     7487 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/charwidth.py
+-rw-rw-r--  2.0 unx     1389 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/platform.py
+-rw-rw-r--  2.0 unx    13504 b- defN 23-Mar-31 19:19 robotframework-6.1b1/src/robot/utils/importer.py
+-rw-rw-r--  2.0 unx      902 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/robotinspect.py
+-rw-rw-r--  2.0 unx     5565 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/utils/robottypes.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/libdoc/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/rebot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/lib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/testdoc/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/common/
+-rw-rw-r--  2.0 unx     4127 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/htmldata/jsonwriter.py
+-rw-rw-r--  2.0 unx     3476 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/htmlfilewriter.py
+-rw-rw-r--  2.0 unx     2535 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/template.py
+-rw-rw-r--  2.0 unx      983 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/__init__.py
+-rw-rw-r--  2.0 unx      138 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/libdoc/print.css
+-rw-rw-r--  2.0 unx    14346 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.css
+-rw-rw-r--  2.0 unx    28636 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.html
+-rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/libdoc/__init__.py
+-rw-rw-r--  2.0 unx     8894 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/libdoc/pygments.css
+-rw-rw-r--  2.0 unx     1341 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/libdoc/doc_formatting.css
+-rw-rw-r--  2.0 unx     4646 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/common.css
+-rw-rw-r--  2.0 unx     3413 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/report.css
+-rw-rw-r--  2.0 unx     6955 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/htmldata/rebot/log.js
+-rw-rw-r--  2.0 unx      699 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/print.css
+-rw-rw-r--  2.0 unx     6510 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/view.js
+-rw-rw-r--  2.0 unx    30836 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/report.html
+-rw-rw-r--  2.0 unx    10023 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/htmldata/rebot/testdata.js
+-rw-rw-r--  2.0 unx     7155 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/util.js
+-rw-rw-r--  2.0 unx    11525 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/htmldata/rebot/model.js
+-rw-rw-r--  2.0 unx    15416 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/htmldata/rebot/log.html
+-rw-rw-r--  2.0 unx     1487 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/fileloading.js
+-rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/rebot/__init__.py
+-rw-rw-r--  2.0 unx      903 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/doc_formatting.css
+-rw-rw-r--  2.0 unx     7390 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/htmldata/rebot/log.css
+-rw-rw-r--  2.0 unx    13667 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jsxcompressor.min.js
+-rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/lib/__init__.py
+-rw-rw-r--  2.0 unx    43881 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.tablesorter.min.js
+-rw-rw-r--  2.0 unx     1524 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.highlight.min.js
+-rw-rw-r--  2.0 unx    89476 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.min.js
+-rw-rw-r--  2.0 unx     6141 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.tmpl.min.js
+-rw-rw-r--  2.0 unx      153 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.css
+-rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/testdoc/__init__.py
+-rw-rw-r--  2.0 unx     9765 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.html
+-rw-rw-r--  2.0 unx      872 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/common/storage.js
+-rw-rw-r--  2.0 unx      373 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/common/js_disabled.css
+-rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/common/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/parser/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/lexer/
+-rw-rw-r--  2.0 unx     6451 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/suitestructure.py
+-rw-rw-r--  2.0 unx     1311 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/__init__.py
+-rw-rw-r--  2.0 unx    14745 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/model/blocks.py
+-rw-rw-r--  2.0 unx     1035 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/model/__init__.py
+-rw-rw-r--  2.0 unx     2355 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/model/visitor.py
+-rw-rw-r--  2.0 unx    44561 b- defN 23-May-05 17:04 robotframework-6.1b1/src/robot/parsing/model/statements.py
+-rw-rw-r--  2.0 unx     3778 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/parser/blockparsers.py
+-rw-rw-r--  2.0 unx     5321 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/parser/parser.py
+-rw-rw-r--  2.0 unx      710 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/parsing/parser/__init__.py
+-rw-rw-r--  2.0 unx     4036 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/parser/fileparser.py
+-rw-rw-r--  2.0 unx     7778 b- defN 23-May-03 20:51 robotframework-6.1b1/src/robot/parsing/lexer/lexer.py
+-rw-rw-r--  2.0 unx    11601 b- defN 23-May-03 20:46 robotframework-6.1b1/src/robot/parsing/lexer/blocklexers.py
+-rw-rw-r--  2.0 unx     5380 b- defN 23-May-03 20:52 robotframework-6.1b1/src/robot/parsing/lexer/context.py
+-rw-rw-r--  2.0 unx     8487 b- defN 23-May-03 21:02 robotframework-6.1b1/src/robot/parsing/lexer/settings.py
+-rw-rw-r--  2.0 unx     9113 b- defN 23-May-03 20:45 robotframework-6.1b1/src/robot/parsing/lexer/tokens.py
+-rw-rw-r--  2.0 unx    10328 b- defN 23-May-03 20:45 robotframework-6.1b1/src/robot/parsing/lexer/statementlexers.py
+-rw-rw-r--  2.0 unx      755 b- defN 23-May-03 20:47 robotframework-6.1b1/src/robot/parsing/lexer/__init__.py
+-rw-rw-r--  2.0 unx     5565 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/lexer/tokenizer.py
+-rw-rw-r--  2.0 unx    71458 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/libraries/XML.py
+-rw-rw-r--  2.0 unx    14289 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Screenshot.py
+-rw-rw-r--  2.0 unx     1104 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/libraries/Easter.py
+-rw-rw-r--  2.0 unx     5960 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libraries/dialogs_py.py
+-rw-rw-r--  2.0 unx    36128 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/String.py
+-rw-rw-r--  2.0 unx    54972 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Telnet.py
+-rw-rw-r--  2.0 unx    28349 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/DateTime.py
+-rw-rw-r--  2.0 unx    10309 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Remote.py
+-rw-rw-r--  2.0 unx    64676 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/OperatingSystem.py
+-rw-rw-r--  2.0 unx    43712 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Collections.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/libraries/__init__.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Reserved.py
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Dialogs.py
+-rw-rw-r--  2.0 unx   187410 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/libraries/BuiltIn.py
+-rw-rw-r--  2.0 unx    44928 b- defN 23-Apr-24 23:30 robotframework-6.1b1/src/robot/libraries/Process.py
+-rw-rw-r--  2.0 unx    22854 b- defN 23-May-05 20:01 robotframework-6.1b1/src/robot/api/interfaces.py
+-rw-rw-r--  2.0 unx    21210 b- defN 23-Apr-04 15:38 robotframework-6.1b1/src/robot/api/parsing.py
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/api/deco.py
+-rw-rw-r--  2.0 unx     4918 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/api/logger.py
+-rw-rw-r--  2.0 unx     4009 b- defN 23-Apr-25 23:34 robotframework-6.1b1/src/robot/api/__init__.py
+-rw-rw-r--  2.0 unx     3140 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/api/exceptions.py
+-rw-rw-r--  2.0 unx     8930 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      108 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/entry_points.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     8685 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/top_level.txt
+305 files, 2338076 bytes uncompressed, 664580 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,901 +1,916 @@
-Filename: robotframework-6.1a1/
+Filename: robotframework-6.1b1/
 Comment: 
 
-Filename: robotframework-6.1a1/src/
+Filename: robotframework-6.1b1/src/
 Comment: 
 
-Filename: robotframework-6.1a1/LICENSE.txt
+Filename: robotframework-6.1b1/LICENSE.txt
 Comment: 
 
-Filename: robotframework-6.1a1/tasks.py
+Filename: robotframework-6.1b1/tasks.py
 Comment: 
 
-Filename: robotframework-6.1a1/BUILD.rst
+Filename: robotframework-6.1b1/BUILD.rst
 Comment: 
 
-Filename: robotframework-6.1a1/COPYRIGHT.txt
+Filename: robotframework-6.1b1/COPYRIGHT.txt
 Comment: 
 
-Filename: robotframework-6.1a1/INSTALL.rst
+Filename: robotframework-6.1b1/INSTALL.rst
 Comment: 
 
-Filename: robotframework-6.1a1/setup.py
+Filename: robotframework-6.1b1/setup.py
 Comment: 
 
-Filename: robotframework-6.1a1/README.rst
+Filename: robotframework-6.1b1/README.rst
 Comment: 
 
-Filename: robotframework-6.1a1/CONTRIBUTING.rst
+Filename: robotframework-6.1b1/CONTRIBUTING.rst
 Comment: 
 
-Filename: robotframework-6.1a1/MANIFEST.in
+Filename: robotframework-6.1b1/MANIFEST.in
 Comment: 
 
-Filename: robotframework-6.1a1/AUTHORS.rst
+Filename: robotframework-6.1b1/AUTHORS.rst
 Comment: 
 
-Filename: robotframework-6.1a1/PKG-INFO
+Filename: robotframework-6.1b1/PKG-INFO
 Comment: 
 
-Filename: robotframework-6.1a1/setup.cfg
+Filename: robotframework-6.1b1/setup.cfg
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/
+Filename: robotframework-6.1b1/src/robot/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robotframework.egg-info/
+Filename: robotframework-6.1b1/src/robotframework.egg-info/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/
+Filename: robotframework-6.1b1/src/robot/result/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/
+Filename: robotframework-6.1b1/src/robot/output/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/
+Filename: robotframework-6.1b1/src/robot/model/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/conf/
+Filename: robotframework-6.1b1/src/robot/conf/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/
+Filename: robotframework-6.1b1/src/robot/variables/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/
+Filename: robotframework-6.1b1/src/robot/libdocpkg/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/
+Filename: robotframework-6.1b1/src/robot/reporting/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/
+Filename: robotframework-6.1b1/src/robot/running/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/
+Filename: robotframework-6.1b1/src/robot/utils/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/
+Filename: robotframework-6.1b1/src/robot/htmldata/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/
+Filename: robotframework-6.1b1/src/robot/parsing/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/
+Filename: robotframework-6.1b1/src/robot/libraries/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/
+Filename: robotframework-6.1b1/src/robot/api/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/pythonpathsetter.py
+Filename: robotframework-6.1b1/src/robot/pythonpathsetter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/rebot.py
+Filename: robotframework-6.1b1/src/robot/rebot.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdoc.py
+Filename: robotframework-6.1b1/src/robot/libdoc.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/errors.py
+Filename: robotframework-6.1b1/src/robot/errors.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/testdoc.py
+Filename: robotframework-6.1b1/src/robot/testdoc.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/__init__.py
+Filename: robotframework-6.1b1/src/robot/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/version.py
+Filename: robotframework-6.1b1/src/robot/version.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/__main__.py
+Filename: robotframework-6.1b1/src/robot/__main__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/run.py
+Filename: robotframework-6.1b1/src/robot/run.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/xmlelementhandlers.py
+Filename: robotframework-6.1b1/src/robot/result/xmlelementhandlers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/executionresult.py
+Filename: robotframework-6.1b1/src/robot/result/executionresult.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/messagefilter.py
+Filename: robotframework-6.1b1/src/robot/result/messagefilter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/suiteteardownfailed.py
+Filename: robotframework-6.1b1/src/robot/result/suiteteardownfailed.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/flattenkeywordmatcher.py
+Filename: robotframework-6.1b1/src/robot/result/flattenkeywordmatcher.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/merger.py
+Filename: robotframework-6.1b1/src/robot/result/merger.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/resultbuilder.py
+Filename: robotframework-6.1b1/src/robot/result/resultbuilder.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/executionerrors.py
+Filename: robotframework-6.1b1/src/robot/result/executionerrors.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/modeldeprecation.py
+Filename: robotframework-6.1b1/src/robot/result/modeldeprecation.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/__init__.py
+Filename: robotframework-6.1b1/src/robot/result/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/keywordremover.py
+Filename: robotframework-6.1b1/src/robot/result/keywordremover.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/visitor.py
+Filename: robotframework-6.1b1/src/robot/result/visitor.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/model.py
+Filename: robotframework-6.1b1/src/robot/result/model.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/result/configurer.py
+Filename: robotframework-6.1b1/src/robot/result/configurer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/console/
+Filename: robotframework-6.1b1/src/robot/output/console/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/listeners.py
+Filename: robotframework-6.1b1/src/robot/output/listeners.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/output.py
+Filename: robotframework-6.1b1/src/robot/output/output.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/listenermethods.py
+Filename: robotframework-6.1b1/src/robot/output/listenermethods.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/pyloggingconf.py
+Filename: robotframework-6.1b1/src/robot/output/pyloggingconf.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/filelogger.py
+Filename: robotframework-6.1b1/src/robot/output/filelogger.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/loggerhelper.py
+Filename: robotframework-6.1b1/src/robot/output/loggerhelper.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/stdoutlogsplitter.py
+Filename: robotframework-6.1b1/src/robot/output/stdoutlogsplitter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/logger.py
+Filename: robotframework-6.1b1/src/robot/output/logger.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/librarylogger.py
+Filename: robotframework-6.1b1/src/robot/output/librarylogger.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/__init__.py
+Filename: robotframework-6.1b1/src/robot/output/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/debugfile.py
+Filename: robotframework-6.1b1/src/robot/output/debugfile.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/xmllogger.py
+Filename: robotframework-6.1b1/src/robot/output/xmllogger.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/listenerarguments.py
+Filename: robotframework-6.1b1/src/robot/output/listenerarguments.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/console/quiet.py
+Filename: robotframework-6.1b1/src/robot/output/console/quiet.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/console/verbose.py
+Filename: robotframework-6.1b1/src/robot/output/console/verbose.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/console/__init__.py
+Filename: robotframework-6.1b1/src/robot/output/console/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/console/dotted.py
+Filename: robotframework-6.1b1/src/robot/output/console/dotted.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/output/console/highlighting.py
+Filename: robotframework-6.1b1/src/robot/output/console/highlighting.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/message.py
+Filename: robotframework-6.1b1/src/robot/model/message.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/stats.py
+Filename: robotframework-6.1b1/src/robot/model/stats.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/testcase.py
+Filename: robotframework-6.1b1/src/robot/model/testcase.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/tags.py
+Filename: robotframework-6.1b1/src/robot/model/tags.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/fixture.py
+Filename: robotframework-6.1b1/src/robot/model/fixture.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/body.py
+Filename: robotframework-6.1b1/src/robot/model/body.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/itemlist.py
+Filename: robotframework-6.1b1/src/robot/model/itemlist.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/testsuite.py
+Filename: robotframework-6.1b1/src/robot/model/testsuite.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/control.py
+Filename: robotframework-6.1b1/src/robot/model/control.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/metadata.py
+Filename: robotframework-6.1b1/src/robot/model/metadata.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/suitestatistics.py
+Filename: robotframework-6.1b1/src/robot/model/suitestatistics.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/modifier.py
+Filename: robotframework-6.1b1/src/robot/model/modifier.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/keyword.py
+Filename: robotframework-6.1b1/src/robot/model/keyword.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/namepatterns.py
+Filename: robotframework-6.1b1/src/robot/model/namepatterns.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/tagsetter.py
+Filename: robotframework-6.1b1/src/robot/model/tagsetter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/__init__.py
+Filename: robotframework-6.1b1/src/robot/model/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/visitor.py
+Filename: robotframework-6.1b1/src/robot/model/visitor.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/totalstatistics.py
+Filename: robotframework-6.1b1/src/robot/model/totalstatistics.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/filter.py
+Filename: robotframework-6.1b1/src/robot/model/filter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/modelobject.py
+Filename: robotframework-6.1b1/src/robot/model/modelobject.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/configurer.py
+Filename: robotframework-6.1b1/src/robot/model/configurer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/statistics.py
+Filename: robotframework-6.1b1/src/robot/model/statistics.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/model/tagstatistics.py
+Filename: robotframework-6.1b1/src/robot/model/tagstatistics.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/conf/settings.py
+Filename: robotframework-6.1b1/src/robot/conf/settings.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/conf/__init__.py
+Filename: robotframework-6.1b1/src/robot/conf/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/conf/languages.py
+Filename: robotframework-6.1b1/src/robot/conf/languages.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/conf/gatherfailed.py
+Filename: robotframework-6.1b1/src/robot/conf/gatherfailed.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/variables.py
+Filename: robotframework-6.1b1/src/robot/variables/variables.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/scopes.py
+Filename: robotframework-6.1b1/src/robot/variables/scopes.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/store.py
+Filename: robotframework-6.1b1/src/robot/variables/store.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/search.py
+Filename: robotframework-6.1b1/src/robot/variables/search.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/replacer.py
+Filename: robotframework-6.1b1/src/robot/variables/replacer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/assigner.py
+Filename: robotframework-6.1b1/src/robot/variables/assigner.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/notfound.py
+Filename: robotframework-6.1b1/src/robot/variables/notfound.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/finders.py
+Filename: robotframework-6.1b1/src/robot/variables/finders.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/__init__.py
+Filename: robotframework-6.1b1/src/robot/variables/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/filesetter.py
+Filename: robotframework-6.1b1/src/robot/variables/filesetter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/evaluation.py
+Filename: robotframework-6.1b1/src/robot/variables/evaluation.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/tablesetter.py
+Filename: robotframework-6.1b1/src/robot/variables/tablesetter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/variables/resolvable.py
+Filename: robotframework-6.1b1/src/robot/variables/resolvable.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/writer.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/writer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/builder.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/builder.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/jsonbuilder.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/jsonbuilder.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/htmlwriter.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/htmlwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/output.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/output.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/jsonwriter.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/jsonwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/xmlwriter.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/xmlwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/standardtypes.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/standardtypes.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/robotbuilder.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/robotbuilder.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/consoleviewer.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/consoleviewer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/datatypes.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/datatypes.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/__init__.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/htmlutils.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/htmlutils.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/model.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/model.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libdocpkg/xmlbuilder.py
+Filename: robotframework-6.1b1/src/robot/libdocpkg/xmlbuilder.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/xunitwriter.py
+Filename: robotframework-6.1b1/src/robot/reporting/xunitwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/jsmodelbuilders.py
+Filename: robotframework-6.1b1/src/robot/reporting/jsmodelbuilders.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/jsbuildingcontext.py
+Filename: robotframework-6.1b1/src/robot/reporting/jsbuildingcontext.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/jswriter.py
+Filename: robotframework-6.1b1/src/robot/reporting/jswriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/stringcache.py
+Filename: robotframework-6.1b1/src/robot/reporting/stringcache.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/__init__.py
+Filename: robotframework-6.1b1/src/robot/reporting/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/resultwriter.py
+Filename: robotframework-6.1b1/src/robot/reporting/resultwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/logreportwriters.py
+Filename: robotframework-6.1b1/src/robot/reporting/logreportwriters.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/jsexecutionresult.py
+Filename: robotframework-6.1b1/src/robot/reporting/jsexecutionresult.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/outputwriter.py
+Filename: robotframework-6.1b1/src/robot/reporting/outputwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/reporting/expandkeywordmatcher.py
+Filename: robotframework-6.1b1/src/robot/reporting/expandkeywordmatcher.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/timeouts/
+Filename: robotframework-6.1b1/src/robot/running/timeouts/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/builder/
+Filename: robotframework-6.1b1/src/robot/running/builder/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/
+Filename: robotframework-6.1b1/src/robot/running/arguments/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/context.py
+Filename: robotframework-6.1b1/src/robot/running/context.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/librarykeywordrunner.py
+Filename: robotframework-6.1b1/src/robot/running/librarykeywordrunner.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/handlers.py
+Filename: robotframework-6.1b1/src/robot/running/handlers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/modelcombiner.py
+Filename: robotframework-6.1b1/src/robot/running/modelcombiner.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/libraryscopes.py
+Filename: robotframework-6.1b1/src/robot/running/libraryscopes.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/signalhandler.py
+Filename: robotframework-6.1b1/src/robot/running/signalhandler.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/userkeywordrunner.py
+Filename: robotframework-6.1b1/src/robot/running/userkeywordrunner.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/bodyrunner.py
+Filename: robotframework-6.1b1/src/robot/running/bodyrunner.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/usererrorhandler.py
+Filename: robotframework-6.1b1/src/robot/running/usererrorhandler.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/suiterunner.py
+Filename: robotframework-6.1b1/src/robot/running/suiterunner.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/status.py
+Filename: robotframework-6.1b1/src/robot/running/status.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/runkwregister.py
+Filename: robotframework-6.1b1/src/robot/running/runkwregister.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/testlibraries.py
+Filename: robotframework-6.1b1/src/robot/running/testlibraries.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/outputcapture.py
+Filename: robotframework-6.1b1/src/robot/running/outputcapture.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/userkeyword.py
+Filename: robotframework-6.1b1/src/robot/running/userkeyword.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/__init__.py
+Filename: robotframework-6.1b1/src/robot/running/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/randomizer.py
+Filename: robotframework-6.1b1/src/robot/running/randomizer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/namespace.py
+Filename: robotframework-6.1b1/src/robot/running/namespace.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/statusreporter.py
+Filename: robotframework-6.1b1/src/robot/running/statusreporter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/handlerstore.py
+Filename: robotframework-6.1b1/src/robot/running/handlerstore.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/dynamicmethods.py
+Filename: robotframework-6.1b1/src/robot/running/dynamicmethods.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/model.py
+Filename: robotframework-6.1b1/src/robot/running/model.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/importer.py
+Filename: robotframework-6.1b1/src/robot/running/importer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/timeouts/posix.py
+Filename: robotframework-6.1b1/src/robot/running/timeouts/posix.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/timeouts/__init__.py
+Filename: robotframework-6.1b1/src/robot/running/timeouts/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/timeouts/windows.py
+Filename: robotframework-6.1b1/src/robot/running/timeouts/windows.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/builder/parsers.py
+Filename: robotframework-6.1b1/src/robot/running/builder/parsers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/builder/transformers.py
+Filename: robotframework-6.1b1/src/robot/running/builder/transformers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/builder/settings.py
+Filename: robotframework-6.1b1/src/robot/running/builder/settings.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/builder/builders.py
+Filename: robotframework-6.1b1/src/robot/running/builder/builders.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/builder/__init__.py
+Filename: robotframework-6.1b1/src/robot/running/builder/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/argumentmapper.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/argumentmapper.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/argumentconverter.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/argumentconverter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/argumentresolver.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/argumentresolver.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/embedded.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/embedded.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/customconverters.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/customconverters.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/typeconverters.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/typeconverters.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/typevalidator.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/typevalidator.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/argumentspec.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/argumentspec.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/argumentparser.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/argumentparser.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/argumentvalidator.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/argumentvalidator.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/running/arguments/__init__.py
+Filename: robotframework-6.1b1/src/robot/running/arguments/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/robotio.py
+Filename: robotframework-6.1b1/src/robot/utils/robotio.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/filereader.py
+Filename: robotframework-6.1b1/src/robot/utils/filereader.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/sortable.py
+Filename: robotframework-6.1b1/src/robot/utils/sortable.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/escaping.py
+Filename: robotframework-6.1b1/src/robot/utils/escaping.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/restreader.py
+Filename: robotframework-6.1b1/src/robot/utils/restreader.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/frange.py
+Filename: robotframework-6.1b1/src/robot/utils/frange.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/connectioncache.py
+Filename: robotframework-6.1b1/src/robot/utils/connectioncache.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/normalizing.py
+Filename: robotframework-6.1b1/src/robot/utils/normalizing.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/markupwriters.py
+Filename: robotframework-6.1b1/src/robot/utils/markupwriters.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/setter.py
+Filename: robotframework-6.1b1/src/robot/utils/setter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/compress.py
+Filename: robotframework-6.1b1/src/robot/utils/compress.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/misc.py
+Filename: robotframework-6.1b1/src/robot/utils/misc.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/dotdict.py
+Filename: robotframework-6.1b1/src/robot/utils/dotdict.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/recommendations.py
+Filename: robotframework-6.1b1/src/robot/utils/recommendations.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/text.py
+Filename: robotframework-6.1b1/src/robot/utils/text.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/unic.py
+Filename: robotframework-6.1b1/src/robot/utils/unic.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/markuputils.py
+Filename: robotframework-6.1b1/src/robot/utils/markuputils.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/robotpath.py
+Filename: robotframework-6.1b1/src/robot/utils/robotpath.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/robottime.py
+Filename: robotframework-6.1b1/src/robot/utils/robottime.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/encoding.py
+Filename: robotframework-6.1b1/src/robot/utils/encoding.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/encodingsniffer.py
+Filename: robotframework-6.1b1/src/robot/utils/encodingsniffer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/argumentparser.py
+Filename: robotframework-6.1b1/src/robot/utils/argumentparser.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/asserts.py
+Filename: robotframework-6.1b1/src/robot/utils/asserts.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/__init__.py
+Filename: robotframework-6.1b1/src/robot/utils/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/application.py
+Filename: robotframework-6.1b1/src/robot/utils/application.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/etreewrapper.py
+Filename: robotframework-6.1b1/src/robot/utils/etreewrapper.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/match.py
+Filename: robotframework-6.1b1/src/robot/utils/match.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/error.py
+Filename: robotframework-6.1b1/src/robot/utils/error.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/robotenv.py
+Filename: robotframework-6.1b1/src/robot/utils/robotenv.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/htmlformatters.py
+Filename: robotframework-6.1b1/src/robot/utils/htmlformatters.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/charwidth.py
+Filename: robotframework-6.1b1/src/robot/utils/charwidth.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/platform.py
+Filename: robotframework-6.1b1/src/robot/utils/platform.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/importer.py
+Filename: robotframework-6.1b1/src/robot/utils/importer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/robotinspect.py
+Filename: robotframework-6.1b1/src/robot/utils/robotinspect.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/utils/robottypes.py
+Filename: robotframework-6.1b1/src/robot/utils/robottypes.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/libdoc/
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/lib/
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/testdoc/
+Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/common/
+Filename: robotframework-6.1b1/src/robot/htmldata/common/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/jsonwriter.py
+Filename: robotframework-6.1b1/src/robot/htmldata/jsonwriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/htmlfilewriter.py
+Filename: robotframework-6.1b1/src/robot/htmldata/htmlfilewriter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/template.py
+Filename: robotframework-6.1b1/src/robot/htmldata/template.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/__init__.py
+Filename: robotframework-6.1b1/src/robot/htmldata/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/libdoc/print.css
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/print.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/libdoc/libdoc.css
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/libdoc/libdoc.html
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.html
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/libdoc/pygments.css
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/libdoc/doc_formatting.css
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/pygments.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/common.css
+Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/doc_formatting.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/report.css
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/common.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/log.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/report.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/print.css
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/log.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/view.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/print.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/report.html
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/view.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/testdata.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/report.html
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/util.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/testdata.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/model.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/util.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/log.html
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/model.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/fileloading.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/log.html
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/doc_formatting.css
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/fileloading.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/rebot/log.css
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/lib/jsxcompressor.min.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/doc_formatting.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/lib/jquery.tablesorter.min.js
+Filename: robotframework-6.1b1/src/robot/htmldata/rebot/log.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/lib/jquery.highlight.min.js
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/jsxcompressor.min.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/lib/jquery.min.js
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/lib/jquery.tmpl.min.js
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.tablesorter.min.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/testdoc/testdoc.css
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.highlight.min.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/testdoc/testdoc.html
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.min.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/common/storage.js
+Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.tmpl.min.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/htmldata/common/js_disabled.css
+Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/model/
+Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/parser/
+Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.html
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/
+Filename: robotframework-6.1b1/src/robot/htmldata/common/storage.js
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/suitestructure.py
+Filename: robotframework-6.1b1/src/robot/htmldata/common/js_disabled.css
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/__init__.py
+Filename: robotframework-6.1b1/src/robot/htmldata/common/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/model/blocks.py
+Filename: robotframework-6.1b1/src/robot/parsing/model/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/model/__init__.py
+Filename: robotframework-6.1b1/src/robot/parsing/parser/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/model/visitor.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/model/statements.py
+Filename: robotframework-6.1b1/src/robot/parsing/suitestructure.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/parser/blockparsers.py
+Filename: robotframework-6.1b1/src/robot/parsing/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/parser/parser.py
+Filename: robotframework-6.1b1/src/robot/parsing/model/blocks.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/parser/__init__.py
+Filename: robotframework-6.1b1/src/robot/parsing/model/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/parser/fileparser.py
+Filename: robotframework-6.1b1/src/robot/parsing/model/visitor.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/lexer.py
+Filename: robotframework-6.1b1/src/robot/parsing/model/statements.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/blocklexers.py
+Filename: robotframework-6.1b1/src/robot/parsing/parser/blockparsers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/context.py
+Filename: robotframework-6.1b1/src/robot/parsing/parser/parser.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/settings.py
+Filename: robotframework-6.1b1/src/robot/parsing/parser/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/tokens.py
+Filename: robotframework-6.1b1/src/robot/parsing/parser/fileparser.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/statementlexers.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/lexer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/__init__.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/blocklexers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/parsing/lexer/tokenizer.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/context.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/XML.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/settings.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Screenshot.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/tokens.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Easter.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/statementlexers.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/dialogs_py.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/String.py
+Filename: robotframework-6.1b1/src/robot/parsing/lexer/tokenizer.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Telnet.py
+Filename: robotframework-6.1b1/src/robot/libraries/XML.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/DateTime.py
+Filename: robotframework-6.1b1/src/robot/libraries/Screenshot.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Remote.py
+Filename: robotframework-6.1b1/src/robot/libraries/Easter.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/OperatingSystem.py
+Filename: robotframework-6.1b1/src/robot/libraries/dialogs_py.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Collections.py
+Filename: robotframework-6.1b1/src/robot/libraries/String.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/__init__.py
+Filename: robotframework-6.1b1/src/robot/libraries/Telnet.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Reserved.py
+Filename: robotframework-6.1b1/src/robot/libraries/DateTime.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Dialogs.py
+Filename: robotframework-6.1b1/src/robot/libraries/Remote.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/BuiltIn.py
+Filename: robotframework-6.1b1/src/robot/libraries/OperatingSystem.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/libraries/Process.py
+Filename: robotframework-6.1b1/src/robot/libraries/Collections.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/interfaces.py
+Filename: robotframework-6.1b1/src/robot/libraries/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/parsing.py
+Filename: robotframework-6.1b1/src/robot/libraries/Reserved.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/deco.py
+Filename: robotframework-6.1b1/src/robot/libraries/Dialogs.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/logger.py
+Filename: robotframework-6.1b1/src/robot/libraries/BuiltIn.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/__init__.py
+Filename: robotframework-6.1b1/src/robot/libraries/Process.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robot/api/exceptions.py
+Filename: robotframework-6.1b1/src/robot/api/interfaces.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robotframework.egg-info/SOURCES.txt
+Filename: robotframework-6.1b1/src/robot/api/parsing.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robotframework.egg-info/entry_points.txt
+Filename: robotframework-6.1b1/src/robot/api/deco.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robotframework.egg-info/dependency_links.txt
+Filename: robotframework-6.1b1/src/robot/api/logger.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robotframework.egg-info/PKG-INFO
+Filename: robotframework-6.1b1/src/robot/api/__init__.py
 Comment: 
 
-Filename: robotframework-6.1a1/src/robotframework.egg-info/top_level.txt
+Filename: robotframework-6.1b1/src/robot/api/exceptions.py
+Comment: 
+
+Filename: robotframework-6.1b1/src/robotframework.egg-info/SOURCES.txt
+Comment: 
+
+Filename: robotframework-6.1b1/src/robotframework.egg-info/entry_points.txt
+Comment: 
+
+Filename: robotframework-6.1b1/src/robotframework.egg-info/dependency_links.txt
+Comment: 
+
+Filename: robotframework-6.1b1/src/robotframework.egg-info/PKG-INFO
+Comment: 
+
+Filename: robotframework-6.1b1/src/robotframework.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `robotframework-6.1a1/LICENSE.txt` & `robotframework-6.1b1/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/tasks.py` & `robotframework-6.1b1/tasks.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/BUILD.rst` & `robotframework-6.1b1/BUILD.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/COPYRIGHT.txt` & `robotframework-6.1b1/COPYRIGHT.txt`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/INSTALL.rst` & `robotframework-6.1b1/INSTALL.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/setup.py` & `robotframework-6.1b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from os.path import abspath, join, dirname
 from setuptools import find_packages, setup
 
 
 # Version number typically updated by running `invoke set-version <version>`.
 # Run `invoke --help set-version` or see tasks.py for details.
-VERSION = '6.1a1'
+VERSION = '6.1b1'
 with open(join(dirname(abspath(__file__)), 'README.rst')) as f:
     LONG_DESCRIPTION = f.read()
     base_url = 'https://github.com/robotframework/robotframework/blob/master'
     for text in ('INSTALL', 'CONTRIBUTING'):
         search = '`<{0}.rst>`__'.format(text)
         replace = '`{0}.rst <{1}/{0}.rst>`__'.format(text, base_url)
         if search not in LONG_DESCRIPTION:
```

## Comparing `robotframework-6.1a1/README.rst` & `robotframework-6.1b1/README.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/CONTRIBUTING.rst` & `robotframework-6.1b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/AUTHORS.rst` & `robotframework-6.1b1/AUTHORS.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/PKG-INFO` & `robotframework-6.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: robotframework
-Version: 6.1a1
+Version: 6.1b1
 Summary: Generic automation framework for acceptance testing and robotic process automation (RPA)
 Home-page: https://robotframework.org
 Author: Pekka Klärck
 Author-email: peke@eliga.fi
 License: Apache License 2.0
 Download-URL: https://pypi.org/project/robotframework
 Project-URL: Source, https://github.com/robotframework/robotframework
 Project-URL: Issue Tracker, https://github.com/robotframework/robotframework/issues
 Project-URL: Documentation, https://robotframework.org/robotframework
-Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1a1.rst
+Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1b1.rst
 Project-URL: Slack, http://slack.robotframework.org
 Project-URL: Twitter, https://twitter.com/robotframework
 Description: Robot Framework
         ===============
         
         .. contents::
            :local:
```

## Comparing `robotframework-6.1a1/src/robot/pythonpathsetter.py` & `robotframework-6.1b1/src/robot/result/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,33 +9,36 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""Module that adds directories needed by Robot to sys.path when imported."""
+"""Implements parsing execution results from XML output files.
 
-import sys
-import fnmatch
-from os.path import abspath, dirname
-
-ROBOTDIR = dirname(abspath(__file__))
-
-def add_path(path, end=False):
-    if not end:
-        remove_path(path)
-        sys.path.insert(0, path)
-    elif not any(fnmatch.fnmatch(p, path) for p in sys.path):
-        sys.path.append(path)
-
-def remove_path(path):
-    sys.path = [p for p in sys.path if not fnmatch.fnmatch(p, path)]
-
-
-# When, for example, robot/run.py is executed as a script, the directory
-# containing the robot module is not added to sys.path automatically but
-# the robot directory itself is. Former is added to allow importing
-# the module and the latter removed to prevent accidentally importing
-# internal modules directly.
-add_path(dirname(ROBOTDIR))
-remove_path(ROBOTDIR)
+The main public API of this package consists of the :func:`~.ExecutionResult`
+factory method, that returns :class:`~.Result` objects, and of the
+:class:`~.ResultVisitor` abstract class, that eases further processing
+the results. It is recommended to import these public entry-points via the
+:mod:`robot.api` package like in the example below.
+
+The model objects defined in the :mod:`robot.result.model` module are also
+part of the public API. They are used inside the :class:`~.Result` object,
+and they can also be inspected and modified as part of the normal test
+execution by using `pre-Rebot modifiers`__ and `listeners`__. These model
+objects are not exposed via :mod:`robot.api`, but they can be imported
+from :mod:`robot.result` if needed.
+
+Example
+-------
+
+.. literalinclude:: /../../doc/api/code_examples/check_test_times.py
+
+__ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#programmatic-modification-of-results
+__ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#listener-interface
+"""
+
+from .executionresult import Result
+from .model import (Break, Continue, Error, For, ForIteration, If, IfBranch, Keyword, Message,
+                    Return, TestCase, TestSuite, Try, TryBranch, While, WhileIteration)
+from .resultbuilder import ExecutionResult, ExecutionResultBuilder
+from .visitor import ResultVisitor
```

## Comparing `robotframework-6.1a1/src/robot/rebot.py` & `robotframework-6.1b1/src/robot/rebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
 This module also provides :func:`rebot` and :func:`rebot_cli` functions
 that can be used programmatically. Other code is for internal usage.
 """
 
 import sys
 
-# Allows running as a script. __name__ check needed with multiprocessing:
-# https://github.com/robotframework/robotframework/issues/1137
-if 'robot' not in sys.modules and __name__ == '__main__':
+if __name__ == '__main__' and 'robot' not in sys.modules:
     import pythonpathsetter
 
 from robot.conf import RebotSettings
 from robot.errors import DataError
 from robot.reporting import ResultWriter
 from robot.output import LOGGER
 from robot.utils import Application
```

## Comparing `robotframework-6.1a1/src/robot/libdoc.py` & `robotframework-6.1b1/src/robot/libdoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,17 @@
 - :func:`~robot.libdocpkg.builder.LibraryDocumentation` as the API to generate
   :class:`~robot.libdocpkg.model.LibraryDoc` instances.
 
 Libdoc itself is implemented in the :mod:`~robot.libdocpkg` package.
 """
 
 import sys
-import os
+from pathlib import Path
 
-# Allows running as a script. __name__ check needed with multiprocessing:
-# https://github.com/robotframework/robotframework/issues/1137
-if 'robot' not in sys.modules and __name__ == '__main__':
+if __name__ == '__main__' and 'robot' not in sys.modules:
     import pythonpathsetter
 
 from robot.utils import Application, seq2str
 from robot.errors import DataError
 from robot.libdocpkg import LibraryDocumentation, ConsoleViewer
 
 
@@ -194,21 +192,21 @@
             = self._get_format_and_specdocformat(format, specdocformat, output)
         if (format == 'HTML'
                 or specdocformat == 'HTML'
                 or format in ('JSON', 'LIBSPEC') and specdocformat != 'RAW'):
             libdoc.convert_docs_to_html()
         libdoc.save(output, format, self._validate_theme(theme, format))
         if not quiet:
-            self.console(os.path.abspath(output))
+            self.console(Path(output).absolute())
 
     def _get_docformat(self, docformat):
         return self._validate('Doc format', docformat, 'ROBOT', 'TEXT', 'HTML', 'REST')
 
     def _get_format_and_specdocformat(self, format, specdocformat, output):
-        extension = os.path.splitext(output)[1][1:]
+        extension = Path(output).suffix[1:]
         format = self._validate('Format', format or extension,
                                 'HTML', 'XML', 'JSON', 'LIBSPEC')
         specdocformat = self._validate('Spec doc format', specdocformat, 'RAW', 'HTML')
         if format == 'HTML' and specdocformat:
             raise DataError("The --specdocformat option is not applicable with "
                             "HTML outputs.")
         return format, specdocformat
```

## Comparing `robotframework-6.1a1/src/robot/errors.py` & `robotframework-6.1b1/src/robot/errors.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/testdoc.py` & `robotframework-6.1b1/src/robot/testdoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,19 @@
 
 Instead of ``python`` it is possible to use also other Python interpreters.
 
 This module also provides :func:`testdoc` and :func:`testdoc_cli` functions
 that can be used programmatically. Other code is for internal usage.
 """
 
-import os.path
 import sys
 import time
+from pathlib import Path
 
-# Allows running as a script. __name__ check needed with multiprocessing:
-# https://github.com/robotframework/robotframework/issues/1137
-if 'robot' not in sys.modules and __name__ == '__main__':
+if __name__ == '__main__' and 'robot' not in sys.modules:
     import pythonpathsetter
 
 from robot.conf import RobotSettings
 from robot.htmldata import HtmlFileWriter, ModelWriter, JsonWriter, TESTDOC
 from robot.running import TestSuiteBuilder
 from robot.utils import (abspath, Application, file_writer, get_link_path,
                          html_escape, html_format, is_list_like, secs_to_timestr,
@@ -182,15 +180,15 @@
             'tests': self._convert_tests(suite),
             'keywords': list(self._convert_keywords((suite.setup, suite.teardown)))
         }
 
     def _get_relative_source(self, source):
         if not source or not self._output_path:
             return ''
-        return get_link_path(source, os.path.dirname(self._output_path))
+        return get_link_path(source, Path(self._output_path).parent)
 
     def _escape(self, item):
         return html_escape(item)
 
     def _html(self, item):
         return html_format(unescape(item))
```

## Comparing `robotframework-6.1a1/src/robot/__init__.py` & `robotframework-6.1b1/src/robot/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/version.py` & `robotframework-6.1b1/src/robot/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  limitations under the License.
 
 import re
 import sys
 
 # Version number typically updated by running `invoke set-version <version>`.
 # Run `invoke --help set-version` or see tasks.py for details.
-VERSION = '6.1a1'
+VERSION = '6.1b1'
 
 
 def get_version(naked=False):
     if naked:
         return re.split('(a|b|rc|.dev)', VERSION)[0]
     return VERSION
```

## Comparing `robotframework-6.1a1/src/robot/__main__.py` & `robotframework-6.1b1/src/robot/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,13 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import sys
 
-# Allows running as a script. __name__ check needed with multiprocessing:
-# https://github.com/robotframework/robotframework/issues/1137
-if 'robot' not in sys.modules and __name__ == '__main__':
+if __name__ == '__main__' and 'robot' not in sys.modules:
     import pythonpathsetter
 
 from robot import run_cli
 
-
-run_cli(sys.argv[1:])
+run_cli()
```

## Comparing `robotframework-6.1a1/src/robot/run.py` & `robotframework-6.1b1/src/robot/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
 This module also provides :func:`run` and :func:`run_cli` functions
 that can be used programmatically. Other code is for internal usage.
 """
 
 import sys
 
-# Allows running as a script. __name__ check needed with multiprocessing:
-# https://github.com/robotframework/robotframework/issues/1137
-if 'robot' not in sys.modules and __name__ == '__main__':
+if __name__ == '__main__' and 'robot' not in sys.modules:
     import pythonpathsetter
 
 from robot.conf import RobotSettings
 from robot.model import ModelModifier
 from robot.output import LOGGER, pyloggingconf
 from robot.reporting import ResultWriter
 from robot.running.builder import TestSuiteBuilder
@@ -285,20 +283,14 @@
                           foritem: deprecated alias for `iteration`
                           name:<pattern>:  flatten matched keywords using same
                                    matching rules as with
                                    `--removekeywords name:<pattern>`
                           tag:<pattern>:  flatten matched keywords using same
                                    matching rules as with
                                    `--removekeywords tag:<pattern>`
-    --listener class *    A class for monitoring test execution. Gets
-                          notifications e.g. when tests start and end.
-                          Arguments to the listener class can be given after
-                          the name using a colon or a semicolon as a separator.
-                          Examples: --listener MyListenerClass
-                                    --listener path/to/Listener.py:arg1:arg2
     --nostatusrc          Sets the return code to zero regardless of failures
                           in test cases. Error codes are returned normally.
     --dryrun              Verifies test data and runs tests so that library
                           keywords are not executed.
  -X --exitonfailure       Stops test execution if any test fails.
     --exitonerror         Stops test execution if any error occurs when parsing
                           test data, importing libraries, and so on.
@@ -309,18 +301,28 @@
                           suites: randomizes suites
                           tests:  randomizes tests
                           none:   no randomization (default)
                           Use syntax `VALUE:SEED` to give a custom random seed.
                           The seed must be an integer.
                           Examples: --randomize all
                                     --randomize tests:1234
-    --prerunmodifier class *  Class to programmatically modify the suite
-                          structure before execution.
-    --prerebotmodifier class *  Class to programmatically modify the result
-                          model before creating reports and logs.
+    --listener listener *  Class or module for monitoring test execution.
+                          Gets notifications e.g. when tests start and end.
+                          Arguments to the listener class can be given after
+                          the name using a colon or a semicolon as a separator.
+                          Examples: --listener MyListener
+                                    --listener path/to/Listener.py:arg1:arg2
+    --prerunmodifier modifier *  Class to programmatically modify the suite
+                          structure before execution. Accepts arguments the
+                          same way as with --listener.
+    --prerebotmodifier modifier *  Class to programmatically modify the result
+                          model before creating reports and logs. Accepts
+                          arguments the same way as with --listener.
+    --parser parser *     Custom parser class or module. Parser classes accept
+                          arguments the same way as with --listener.
     --console type        How to report execution on the console.
                           verbose:  report every suite and test (default)
                           dotted:   only show `.` for passed test, `s` for
                                     skipped tests, and `F` for failed tests
                           quiet:    no output except for errors and warnings
                           none:     no output whatsoever
  -. --dotted              Shortcut for `--console dotted`.
@@ -411,30 +413,31 @@
 $ robot tests.robot
 """
 
 
 class RobotFramework(Application):
 
     def __init__(self):
-        Application.__init__(self, USAGE, arg_limits=(1,), env_options='ROBOT_OPTIONS',
-                             logger=LOGGER)
+        super().__init__(USAGE, arg_limits=(1,), env_options='ROBOT_OPTIONS',
+                         logger=LOGGER)
 
     def main(self, datasources, **options):
         try:
             settings = RobotSettings(options)
         except:
             LOGGER.register_console_logger(stdout=options.get('stdout'),
                                            stderr=options.get('stderr'))
             raise
         LOGGER.register_console_logger(**settings.console_output_config)
         LOGGER.info(f'Settings:\n{settings}')
         if settings.pythonpath:
             sys.path = settings.pythonpath + sys.path
         builder = TestSuiteBuilder(settings.suite_names,
                                    included_extensions=settings.extension,
+                                   custom_parsers=settings.parsers,
                                    rpa=settings.rpa,
                                    lang=settings.languages,
                                    allow_empty_suite=settings.run_empty_suite)
         suite = builder.build(*datasources)
         settings.rpa = suite.rpa
         if settings.pre_run_modifiers:
             suite.visit(ModelModifier(settings.pre_run_modifiers,
```

## Comparing `robotframework-6.1a1/src/robot/result/xmlelementhandlers.py` & `robotframework-6.1b1/src/robot/result/xmlelementhandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,16 +186,20 @@
 
 @ElementHandler.register
 class WhileHandler(ElementHandler):
     tag = 'while'
     children = frozenset(('iter', 'status', 'doc', 'msg', 'kw'))
 
     def start(self, elem, result):
-        return result.body.create_while(condition=elem.get('condition'),
-                                        limit=elem.get('limit'))
+        return result.body.create_while(
+            condition=elem.get('condition'),
+            limit=elem.get('limit'),
+            on_limit=elem.get('on_limit'),
+            on_limit_message=elem.get('on_limit_message')
+        )
 
 
 @ElementHandler.register
 class IterationHandler(ElementHandler):
     tag = 'iter'
     children = frozenset(('var', 'doc', 'status', 'kw', 'if', 'for', 'msg', 'try',
                           'while', 'return', 'break', 'continue', 'error'))
```

## Comparing `robotframework-6.1a1/src/robot/result/executionresult.py` & `robotframework-6.1b1/src/robot/result/executionresult.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/messagefilter.py` & `robotframework-6.1b1/src/robot/result/messagefilter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/suiteteardownfailed.py` & `robotframework-6.1b1/src/robot/result/suiteteardownfailed.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/flattenkeywordmatcher.py` & `robotframework-6.1b1/src/robot/result/flattenkeywordmatcher.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/merger.py` & `robotframework-6.1b1/src/robot/result/merger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/resultbuilder.py` & `robotframework-6.1b1/src/robot/result/resultbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/executionerrors.py` & `robotframework-6.1b1/src/robot/result/executionerrors.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/modeldeprecation.py` & `robotframework-6.1b1/src/robot/result/modeldeprecation.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/keywordremover.py` & `robotframework-6.1b1/src/robot/result/keywordremover.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             self._clear_content(kw)
 
 
 class ByTagKeywordRemover(_KeywordRemover):
 
     def __init__(self, pattern):
         _KeywordRemover.__init__(self)
-        self._pattern = TagPattern(pattern)
+        self._pattern = TagPattern.from_string(pattern)
 
     def start_keyword(self, kw):
         if self._pattern.match(kw.tags) and not self._warning_or_error(kw):
             self._clear_content(kw)
 
 
 class _LoopItemsRemover(_KeywordRemover):
```

## Comparing `robotframework-6.1a1/src/robot/result/visitor.py` & `robotframework-6.1b1/src/robot/result/visitor.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/result/model.py` & `robotframework-6.1b1/src/robot/result/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,17 +228,18 @@
 
 @Body.register
 class While(model.While, StatusMixin, DeprecatedAttributesMixin):
     iterations_class = Iterations
     iteration_class = WhileIteration
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, condition=None, limit=None, parent=None, status='FAIL',
+    def __init__(self, condition=None, limit=None, on_limit=None,
+                 on_limit_message=None, parent=None, status='FAIL',
                  starttime=None, endtime=None, doc=''):
-        super().__init__(condition, limit, parent)
+        super().__init__(condition, limit, on_limit, on_limit_message, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
     @setter
     def body(self, iterations):
@@ -248,14 +249,18 @@
     @deprecated
     def name(self):
         parts = []
         if self.condition:
             parts.append(self.condition)
         if self.limit:
             parts.append(f'limit={self.limit}')
+        if self.on_limit:
+            parts.append(f'on_limit={self.on_limit}')
+        if self.on_limit_message:
+            parts.append(f'on_limit_message={self.on_limit_message}')
         return ' | '.join(parts)
 
 
 class IfBranch(model.IfBranch, StatusMixin, DeprecatedAttributesMixin):
     body_class = Body
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
```

## Comparing `robotframework-6.1a1/src/robot/result/configurer.py` & `robotframework-6.1b1/src/robot/result/configurer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/listeners.py` & `robotframework-6.1b1/src/robot/output/listeners.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/output.py` & `robotframework-6.1b1/src/robot/output/output.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/listenermethods.py` & `robotframework-6.1b1/src/robot/output/listenermethods.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/pyloggingconf.py` & `robotframework-6.1b1/src/robot/output/pyloggingconf.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/filelogger.py` & `robotframework-6.1b1/src/robot/output/filelogger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/loggerhelper.py` & `robotframework-6.1b1/src/robot/output/loggerhelper.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/stdoutlogsplitter.py` & `robotframework-6.1b1/src/robot/output/stdoutlogsplitter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/logger.py` & `robotframework-6.1b1/src/robot/output/logger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/librarylogger.py` & `robotframework-6.1b1/src/robot/output/librarylogger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/__init__.py` & `robotframework-6.1b1/src/robot/output/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/debugfile.py` & `robotframework-6.1b1/src/robot/output/debugfile.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/xmllogger.py` & `robotframework-6.1b1/src/robot/output/xmllogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,17 @@
     def end_try_branch(self, branch):
         self._write_status(branch)
         self._writer.end('branch')
 
     def start_while(self, while_):
         self._writer.start('while', attrs={
             'condition': while_.condition,
-            'limit': while_.limit
+            'limit': while_.limit,
+            'on_limit': while_.on_limit,
+            'on_limit_message': while_.on_limit_message
         })
         self._writer.element('doc', while_.doc)
 
     def end_while(self, while_):
         self._write_status(while_)
         self._writer.end('while')
```

## Comparing `robotframework-6.1a1/src/robot/output/listenerarguments.py` & `robotframework-6.1b1/src/robot/output/listenerarguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 class StartKeywordArguments(_ListenerArgumentsFromItem):
     _attribute_names = ('doc', 'assign', 'tags', 'lineno', 'type', 'status', 'starttime')
     _type_attributes = {
         BodyItem.FOR: ('variables', 'flavor', 'values'),
         BodyItem.IF: ('condition',),
         BodyItem.ELSE_IF: ('condition',),
         BodyItem.EXCEPT: ('patterns', 'pattern_type', 'variable'),
-        BodyItem.WHILE: ('condition', 'limit'),
+        BodyItem.WHILE: ('condition', 'limit', 'on_limit_message'),
         BodyItem.RETURN: ('values',),
         BodyItem.ITERATION: ('variables',)
     }
     _for_flavor_attributes = {
         'IN ENUMERATE': ('start',),
         'IN ZIP': ('mode', 'fill')
     }
```

## Comparing `robotframework-6.1a1/src/robot/output/console/quiet.py` & `robotframework-6.1b1/src/robot/output/console/quiet.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/console/verbose.py` & `robotframework-6.1b1/src/robot/output/console/verbose.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/console/__init__.py` & `robotframework-6.1b1/src/robot/output/console/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/console/dotted.py` & `robotframework-6.1b1/src/robot/output/console/dotted.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/output/console/highlighting.py` & `robotframework-6.1b1/src/robot/output/console/highlighting.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/message.py` & `robotframework-6.1b1/src/robot/model/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         """Returns the message content as HTML."""
         return self.message if self.html else html_escape(self.message)
 
     @property
     def id(self):
         if not self.parent:
             return 'm1'
-        return '%s-m%d' % (self.parent.id, self.parent.messages.index(self) + 1)
+        messages = self.parent.messages
+        index = messages.index(self) if self in messages else len(messages)
+        return f'{self.parent.id}-m{index + 1}'
 
     def visit(self, visitor):
         """:mod:`Visitor interface <robot.model.visitor>` entry-point."""
         visitor.visit_message(self)
 
     def __str__(self):
         return self.message
```

## Comparing `robotframework-6.1a1/src/robot/model/stats.py` & `robotframework-6.1b1/src/robot/model/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,11 +161,11 @@
         return (not self.combined, self._norm_name)
 
 
 class CombinedTagStat(TagStat):
 
     def __init__(self, pattern, name=None, doc='', links=None):
         TagStat.__init__(self, name or pattern, doc, links, combined=pattern)
-        self.pattern = TagPattern(pattern)
+        self.pattern = TagPattern.from_string(pattern)
 
     def match(self, tags):
         return self.pattern.match(tags)
```

## Comparing `robotframework-6.1a1/src/robot/model/testcase.py` & `robotframework-6.1b1/src/robot/model/testcase.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,59 +9,67 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from pathlib import Path
+from typing import Any, Iterable, Mapping, Sequence, Type, TYPE_CHECKING
+
 from robot.utils import setter
 
 from .body import Body
 from .fixture import create_fixture
 from .itemlist import ItemList
 from .keyword import Keyword, Keywords
 from .modelobject import ModelObject
 from .tags import Tags
 
+if TYPE_CHECKING:
+    from .testsuite import TestSuite
+    from .visitor import SuiteVisitor
+
 
 class TestCase(ModelObject):
     """Base model for a single test case.
 
     Extended by :class:`robot.running.model.TestCase` and
     :class:`robot.result.model.TestCase`.
     """
     body_class = Body
     fixture_class = Keyword
     repr_args = ('name',)
     __slots__ = ['parent', 'name', 'doc', 'timeout', 'lineno', '_setup', '_teardown']
 
-    def __init__(self, name='', doc='', tags=None, timeout=None, lineno=None,
-                 parent=None):
+    def __init__(self, name: str = '', doc: str = '', tags: Sequence[str] = (),
+                 timeout: 'str|None' = None, lineno: 'int|None' = None,
+                 parent: 'TestSuite|None' = None):
         self.name = name
         self.doc = doc
         self.tags = tags
         self.timeout = timeout
         self.lineno = lineno
         self.parent = parent
-        self.body = None
-        self._setup = None
-        self._teardown = None
+        self.body = []
+        self._setup: 'Keyword|None' = None
+        self._teardown: 'Keyword|None' = None
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Iterable[Keyword|Mapping]') -> Body:
         """Test body as a :class:`~robot.model.body.Body` object."""
         return self.body_class(self, body)
 
     @setter
-    def tags(self, tags):
+    def tags(self, tags: Sequence[str]) -> Tags:
         """Test tags as a :class:`~.model.tags.Tags` object."""
         return Tags(tags)
 
     @property
-    def setup(self):
+    def setup(self) -> Keyword:
         """Test setup as a :class:`~.model.keyword.Keyword` object.
 
         This attribute is a ``Keyword`` object also when a test has no setup
         but in that case its truth value is ``False``.
 
         Setup can be modified by setting attributes directly::
 
@@ -77,104 +85,106 @@
         It will automatically recreate the underlying ``Keyword`` object::
 
             test.setup = None
 
         New in Robot Framework 4.0. Earlier setup was accessed like
         ``test.keywords.setup``.
         """
-        if self._setup is None and self:
+        if self._setup is None:
             self._setup = create_fixture(None, self, Keyword.SETUP)
         return self._setup
 
     @setup.setter
-    def setup(self, setup):
+    def setup(self, setup: 'Keyword|Mapping|None'):
         self._setup = create_fixture(setup, self, Keyword.SETUP)
 
     @property
-    def has_setup(self):
+    def has_setup(self) -> bool:
         """Check does a suite have a setup without creating a setup object.
 
         A difference between using ``if test.has_setup:`` and ``if test.setup:``
         is that accessing the :attr:`setup` attribute creates a :class:`Keyword`
         object representing the setup even when the test actually does not have
         one. This typically does not matter, but with bigger suite structures
         containing a huge about of tests it can have an effect on memory usage.
 
         New in Robot Framework 5.0.
         """
         return bool(self._setup)
 
     @property
-    def teardown(self):
+    def teardown(self) -> Keyword:
         """Test teardown as a :class:`~.model.keyword.Keyword` object.
 
         See :attr:`setup` for more information.
         """
-        if self._teardown is None and self:
+        if self._teardown is None:
             self._teardown = create_fixture(None, self, Keyword.TEARDOWN)
         return self._teardown
 
     @teardown.setter
-    def teardown(self, teardown):
+    def teardown(self, teardown: 'Keyword|Mapping|None'):
         self._teardown = create_fixture(teardown, self, Keyword.TEARDOWN)
 
     @property
-    def has_teardown(self):
+    def has_teardown(self) -> bool:
         """Check does a test have a teardown without creating a teardown object.
 
         See :attr:`has_setup` for more information.
 
         New in Robot Framework 5.0.
         """
         return bool(self._teardown)
 
     @property
-    def keywords(self):
+    def keywords(self) -> Keywords:
         """Deprecated since Robot Framework 4.0
 
         Use :attr:`body`, :attr:`setup` or :attr:`teardown` instead.
         """
         keywords = [self.setup] + list(self.body) + [self.teardown]
         return Keywords(self, [kw for kw in keywords if kw])
 
     @keywords.setter
     def keywords(self, keywords):
         Keywords.raise_deprecation_error()
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Test case id in format like ``s1-t3``.
 
         See :attr:`TestSuite.id <robot.model.testsuite.TestSuite.id>` for
         more information.
         """
         if not self.parent:
             return 't1'
-        return '%s-t%d' % (self.parent.id, self.parent.tests.index(self)+1)
+        tests = self.parent.tests
+        index = tests.index(self) if self in tests else len(tests)
+        return f'{self.parent.id}-t{index + 1}'
 
     @property
-    def longname(self):
+    def longname(self) -> str:
         """Test name prefixed with the long name of the parent suite."""
         if not self.parent:
             return self.name
-        return '%s.%s' % (self.parent.longname, self.name)
+        return f'{self.parent.longname}.{self.name}'
 
     @property
-    def source(self):
+    def source(self) -> 'Path|None':
         return self.parent.source if self.parent is not None else None
 
-    def visit(self, visitor):
+    def visit(self, visitor: 'SuiteVisitor'):
         """:mod:`Visitor interface <robot.model.visitor>` entry-point."""
         visitor.visit_test(self)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
-    def to_dict(self):
-        data = {'name': self.name}
+    def to_dict(self) -> 'dict[str, Any]':
+        data: 'dict[str, Any]' = {'name': self.name}
         if self.doc:
             data['doc'] = self.doc
         if self.tags:
             data['tags'] = list(self.tags)
         if self.timeout:
             data['timeout'] = self.timeout
         if self.lineno:
@@ -183,18 +193,21 @@
             data['setup'] = self.setup.to_dict()
         if self.has_teardown:
             data['teardown'] = self.teardown.to_dict()
         data['body'] = self.body.to_dicts()
         return data
 
 
-class TestCases(ItemList):
+class TestCases(ItemList[TestCase]):
     __slots__ = []
 
-    def __init__(self, test_class=TestCase, parent=None, tests=None):
+    def __init__(self, test_class: Type[TestCase] = TestCase,
+                 parent: 'TestSuite|None' = None,
+                 tests: 'Sequence[TestCase|Mapping]' = ()):
         super().__init__(test_class, {'parent': parent}, tests)
 
     def _check_type_and_set_attrs(self, test):
         test = super()._check_type_and_set_attrs(test)
-        for visitor in test.parent._visitors:
-            test.visit(visitor)
+        if test.parent:
+            for visitor in test.parent._visitors:
+                test.visit(visitor)
         return test
```

## Comparing `robotframework-6.1a1/src/robot/model/fixture.py` & `robotframework-6.1b1/src/robot/model/fixture.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from collections.abc import Mapping
 
+from .keyword import Keyword
 
-def create_fixture(fixture, parent, fixture_type):
+
+def create_fixture(fixture, parent, fixture_type) -> Keyword:
     # TestCase and TestSuite have 'fixture_class', Keyword doesn't.
     fixture_class = getattr(parent, 'fixture_class', parent.__class__)
     if isinstance(fixture, fixture_class):
         return fixture.config(parent=parent, type=fixture_type)
     if isinstance(fixture, Mapping):
         return fixture_class.from_dict(fixture).config(parent=parent, type=fixture_type)
     if fixture is None:
```

## Comparing `robotframework-6.1a1/src/robot/model/body.py` & `robotframework-6.1b1/src/robot/model/body.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,17 @@
         if getattr(parent, 'has_setup', False):
             steps.append(parent.setup)
         if hasattr(parent, 'body'):
             steps.extend(step for step in parent.body.flatten()
                          if step.type != self.MESSAGE)
         if getattr(parent, 'has_teardown', False):
             steps.append(parent.teardown)
-        my_id = steps.index(self) + 1
-        return f'{parent.id}-k{my_id}'
+        index = steps.index(self) if self in steps else len(steps)
+        parent_id = parent.id
+        return f'{parent_id}-k{index + 1}' if parent_id else f'k{index + 1}'
 
     def to_dict(self):
         raise NotImplementedError
 
 
 class BaseBody(ItemList):
     """Base class for Body and Branches objects."""
@@ -148,15 +149,15 @@
     def create_break(self, *args, **kwargs):
         return self._create(self.break_class, 'create_break', args, kwargs)
 
     def create_message(self, *args, **kwargs):
         return self._create(self.message_class, 'create_message', args, kwargs)
 
     def create_error(self, *args, **kwargs):
-        return self._create(self.error_class, 'create_message', args, kwargs)
+        return self._create(self.error_class, 'create_error', args, kwargs)
 
     def filter(self, keywords=None, messages=None, predicate=None):
         """Filter body items based on type and/or custom predicate.
 
         To include or exclude items based on types, give matching arguments
         ``True`` or ``False`` values. For example, to include only keywords,
         use ``body.filter(keywords=True)`` and to exclude messages use
```

## Comparing `robotframework-6.1a1/src/robot/model/itemlist.py` & `robotframework-6.1b1/src/robot/model/itemlist.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,31 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from collections.abc import MutableSequence
 from functools import total_ordering
+from collections.abc import Mapping
+from typing import (Iterable, Iterator, MutableSequence, overload, TYPE_CHECKING,
+                    Type, TypeVar)
 
 from robot.utils import type_name
 
+if TYPE_CHECKING:
+    from .visitor import SuiteVisitor
+
+
+T = TypeVar('T')
+Self = TypeVar('Self', bound='ItemList')
+
 
 @total_ordering
-class ItemList(MutableSequence):
+class ItemList(MutableSequence[T]):
     """List of items of a certain enforced type.
 
     New items can be created using the :meth:`create` method and existing items
     added using the common list methods like :meth:`append` or :meth:`insert`.
     In addition to the common type, items can have certain common and
     automatically assigned attributes.
 
@@ -32,165 +41,182 @@
     actual items are generated based on them automatically. If the type has
     a ``from_dict`` class method, it is used, and otherwise dictionary data is
     passed to the type as keyword arguments.
     """
 
     __slots__ = ['_item_class', '_common_attrs', '_items']
 
-    def __init__(self, item_class, common_attrs=None, items=None):
+    def __init__(self, item_class: Type[T],
+                 common_attrs: 'Mapping|None' = None,
+                 items: 'Iterable[T|Mapping]' = ()):
         self._item_class = item_class
         self._common_attrs = common_attrs
-        self._items = []
+        self._items: 'list[T]' = []
         if items:
             self.extend(items)
 
-    def create(self, *args, **kwargs):
+    def create(self, *args, **kwargs) -> T:
         """Create a new item using the provided arguments."""
         return self.append(self._item_class(*args, **kwargs))
 
-    def append(self, item):
+    def append(self, item: 'T|Mapping'):
         item = self._check_type_and_set_attrs(item)
         self._items.append(item)
         return item
 
-    def _check_type_and_set_attrs(self, item):
+    def _check_type_and_set_attrs(self, item: 'T|Mapping') -> T:
         if not isinstance(item, self._item_class):
-            if isinstance(item, dict):
+            if isinstance(item, Mapping):
                 item = self._item_from_dict(item)
             else:
                 raise TypeError(f'Only {type_name(self._item_class)} objects '
                                 f'accepted, got {type_name(item)}.')
         if self._common_attrs:
             for attr, value in self._common_attrs.items():
                 setattr(item, attr, value)
         return item
 
-    def _item_from_dict(self, data):
+    def _item_from_dict(self, data: Mapping) -> T:
         if hasattr(self._item_class, 'from_dict'):
-            return self._item_class.from_dict(data)
+            return self._item_class.from_dict(data)    # type: ignore
         return self._item_class(**data)
 
-    def extend(self, items):
+    def extend(self, items: 'Iterable[T|Mapping]'):
         self._items.extend(self._check_type_and_set_attrs(i) for i in items)
 
-    def insert(self, index, item):
+    def insert(self, index: int, item: 'T|Mapping'):
         item = self._check_type_and_set_attrs(item)
         self._items.insert(index, item)
 
-    def index(self, item, *start_and_end):
+    def index(self, item: T, *start_and_end) -> int:
         return self._items.index(item, *start_and_end)
 
     def clear(self):
         self._items = []
 
-    def visit(self, visitor):
+    def visit(self, visitor: 'SuiteVisitor'):
         for item in self:
-            item.visit(visitor)
+            item.visit(visitor)    # type: ignore
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[T]:
         index = 0
         while index < len(self._items):
             yield self._items[index]
             index += 1
 
+    @overload
+    def __getitem__(self, index: int) -> T:
+        ...
+
+    @overload
+    def __getitem__(self: Self, index: slice) -> Self:
+        ...
+
     def __getitem__(self, index):
         if isinstance(index, slice):
             return self._create_new_from(self._items[index])
         return self._items[index]
 
-    def _create_new_from(self, items):
+    def _create_new_from(self: Self, items: Iterable[T]) -> Self:
         # Cannot pass common_attrs directly to new object because all
         # subclasses don't have compatible __init__.
         new = type(self)(self._item_class)
         new._common_attrs = self._common_attrs
         new.extend(items)
         return new
 
+    @overload
+    def __setitem__(self, index: int, item: 'T|Mapping'):
+        ...
+
+    @overload
+    def __setitem__(self, index: slice, item: 'Iterable[T|Mapping]'):
+        ...
+
     def __setitem__(self, index, item):
         if isinstance(index, slice):
-            item = [self._check_type_and_set_attrs(i) for i in item]
+            self._items[index] = [self._check_type_and_set_attrs(i) for i in item]
         else:
-            item = self._check_type_and_set_attrs(item)
-        self._items[index] = item
+            self._items[index] = self._check_type_and_set_attrs(item)
 
-    def __delitem__(self, index):
+    def __delitem__(self, index: 'int|slice'):
         del self._items[index]
 
-    def __contains__(self, item):
+    def __contains__(self, item: object) -> bool:
         return item in self._items
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._items)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(list(self))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         class_name = type(self).__name__
         item_name = self._item_class.__name__
         return f'{class_name}(item_class={item_name}, items={self._items})'
 
-    def count(self, item):
+    def count(self, item: T) -> int:
         return self._items.count(item)
 
-    def sort(self):
-        self._items.sort()
+    def sort(self, **config):
+        self._items.sort(**config)
 
     def reverse(self):
         self._items.reverse()
 
-    def __reversed__(self):
+    def __reversed__(self) -> Iterator[T]:
         index = 0
         while index < len(self._items):
             yield self._items[len(self._items) - index - 1]
             index += 1
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return (isinstance(other, ItemList)
                 and self._is_compatible(other)
                 and self._items == other._items)
 
-    def _is_compatible(self, other):
+    def _is_compatible(self, other) -> bool:
         return (self._item_class is other._item_class
                 and self._common_attrs == other._common_attrs)
 
-    def __lt__(self, other):
+    def __lt__(self, other: 'ItemList[T]') -> bool:
         if not isinstance(other, ItemList):
             raise TypeError(f'Cannot order ItemList and {type_name(other)}.')
         if not self._is_compatible(other):
             raise TypeError('Cannot order incompatible ItemLists.')
         return self._items < other._items
 
-    def __add__(self, other):
+    def __add__(self: Self, other: 'ItemList[T]') -> Self:
         if not isinstance(other, ItemList):
             raise TypeError(f'Cannot add ItemList and {type_name(other)}.')
         if not self._is_compatible(other):
             raise TypeError('Cannot add incompatible ItemLists.')
         return self._create_new_from(self._items + other._items)
 
-    def __iadd__(self, other):
+    def __iadd__(self: Self, other: Iterable[T]) -> Self:
         if isinstance(other, ItemList) and not self._is_compatible(other):
             raise TypeError('Cannot add incompatible ItemLists.')
         self.extend(other)
         return self
 
-    def __mul__(self, other):
-        return self._create_new_from(self._items * other)
+    def __mul__(self: Self, count: int) -> Self:
+        return self._create_new_from(self._items * count)
 
-    def __imul__(self, other):
-        self._items *= other
+    def __imul__(self: Self, count: int) -> Self:
+        self._items *= count
         return self
 
-    def __rmul__(self, other):
-        return self * other
+    def __rmul__(self: Self, count: int) -> Self:
+        return self * count
 
-    def to_dicts(self):
+    def to_dicts(self) -> 'list[dict]':
         """Return list of items converted to dictionaries.
 
         Items are converted to dictionaries using the ``to_dict`` method, if
         they have it, or the built-in ``vars()``.
 
         New in Robot Framework 6.1.
         """
         if not hasattr(self._item_class, 'to_dict'):
             return [vars(item) for item in self]
-        return [item.to_dict() for item in self]
+        return [item.to_dict() for item in self]    # type: ignore
```

## Comparing `robotframework-6.1a1/src/robot/model/testsuite.py` & `robotframework-6.1b1/src/robot/model/testsuite.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,119 +9,122 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from collections.abc import Mapping
 from pathlib import Path
+from typing import Any, Iterator, Sequence, Type
 
 from robot.utils import setter
 
 from .configurer import SuiteConfigurer
 from .filter import Filter, EmptySuiteRemover
 from .fixture import create_fixture
 from .itemlist import ItemList
 from .keyword import Keyword, Keywords
 from .metadata import Metadata
 from .modelobject import ModelObject
 from .tagsetter import TagSetter
 from .testcase import TestCase, TestCases
+from .visitor import SuiteVisitor
 
 
 class TestSuite(ModelObject):
     """Base model for single suite.
 
     Extended by :class:`robot.running.model.TestSuite` and
     :class:`robot.result.model.TestSuite`.
     """
     test_class = TestCase    #: Internal usage only.
     fixture_class = Keyword  #: Internal usage only.
     repr_args = ('name',)
-    __slots__ = ['parent', '_name', 'doc', '_setup', '_teardown',  'rpa',
-                 '_my_visitors']
+    __slots__ = ['parent', '_name', 'doc', '_setup', '_teardown', 'rpa', '_my_visitors']
 
-    def __init__(self, name: str = '', doc: str = '', metadata: dict = None,
-                 source: Path = None, rpa: bool = False, parent: 'TestSuite' = None):
+    def __init__(self, name: str = '', doc: str = '', metadata: 'Mapping|None' = None,
+                 source: 'Path|str|None' = None, rpa: 'bool|None' = None,
+                 parent: 'TestSuite|None' = None):
         self._name = name
         self.doc = doc
         self.metadata = metadata
         self.source = source
         self.parent = parent
-        self.rpa = rpa        #: ``True`` when RPA mode is enabled.
-        self.suites = None
-        self.tests = None
-        self._setup = None
-        self._teardown = None
-        self._my_visitors = []
+        self.rpa = rpa
+        self.suites = []
+        self.tests = []
+        self._setup: 'Keyword|None' = None
+        self._teardown: 'Keyword|None' = None
+        self._my_visitors: 'list[SuiteVisitor]' = []
 
     @staticmethod
-    def name_from_source(source: Path):
+    def name_from_source(source: 'Path|str|None') -> str:
         if not source:
             return ''
         if not isinstance(source, Path):
             source = Path(source)
         name = source.name if source.is_dir() else source.stem
         if '__' in name:
             name = name.split('__', 1)[1] or name
         name = name.replace('_', ' ').strip()
         return name.title() if name.islower() else name
 
     @property
-    def _visitors(self):
+    def _visitors(self) -> 'list[SuiteVisitor]':
         parent_visitors = self.parent._visitors if self.parent else []
         return self._my_visitors + parent_visitors
 
     @property
-    def name(self):
-        """Test suite name.
+    def name(self) -> str:
+        """Suite name.
 
         If name is not set, it is constructed from source. If source is not set,
-        name is constructed from child suite names or.
+        name is constructed from child suite names by concatenating them with
+        `` & ``. If there are no child suites, name is an empty string.
         """
         return (self._name
                 or self.name_from_source(self.source)
                 or ' & '.join(s.name for s in self.suites))
 
     @name.setter
-    def name(self, name):
+    def name(self, name: str):
         self._name = name
 
     @setter
-    def source(self, source):
+    def source(self, source: 'Path|str|None') -> 'Path|None':
         return source if isinstance(source, (Path, type(None))) else Path(source)
 
     @property
-    def longname(self):
+    def longname(self) -> str:
         """Suite name prefixed with the long name of the parent suite."""
         if not self.parent:
             return self.name
         return f'{self.parent.longname}.{self.name}'
 
     @setter
-    def metadata(self, metadata):
-        """Free test suite metadata as a dictionary."""
+    def metadata(self, metadata: 'Mapping|None') -> Metadata:
+        """Free suite metadata as dictionary-like ``Metadata`` object."""
         return Metadata(metadata)
 
     @setter
-    def suites(self, suites):
-        """Child suites as a :class:`~.TestSuites` object."""
+    def suites(self, suites: 'Sequence[TestSuite|Mapping]') -> 'TestSuites':
         return TestSuites(self.__class__, self, suites)
 
     @setter
-    def tests(self, tests):
-        """Tests as a :class:`~.TestCases` object."""
+    def tests(self, tests: 'Sequence[TestCase|Mapping]') -> TestCases:
         return TestCases(self.test_class, self, tests)
 
     @property
-    def setup(self):
-        """Suite setup as a :class:`~.model.keyword.Keyword` object.
+    def setup(self) -> Keyword:
+        """Suite setup.
 
         This attribute is a ``Keyword`` object also when a suite has no setup
-        but in that case its truth value is ``False``.
+        but in that case its truth value is ``False``. The preferred way to
+        check does a suite have a setup is using :attr:`has_setup`.
 
         Setup can be modified by setting attributes directly::
 
             suite.setup.name = 'Example'
             suite.setup.args = ('First', 'Second')
 
         Alternatively the :meth:`config` method can be used to set multiple
@@ -133,130 +136,133 @@
         It will automatically recreate the underlying ``Keyword`` object::
 
             suite.setup = None
 
         New in Robot Framework 4.0. Earlier setup was accessed like
         ``suite.keywords.setup``.
         """
-        if self._setup is None and self:
+        if self._setup is None:
             self._setup = create_fixture(None, self, Keyword.SETUP)
         return self._setup
 
     @setup.setter
-    def setup(self, setup):
+    def setup(self, setup: 'Keyword|Mapping|None'):
         self._setup = create_fixture(setup, self, Keyword.SETUP)
 
     @property
-    def has_setup(self):
+    def has_setup(self) -> bool:
         """Check does a suite have a setup without creating a setup object.
 
         A difference between using ``if suite.has_setup:`` and ``if suite.setup:``
         is that accessing the :attr:`setup` attribute creates a :class:`Keyword`
         object representing the setup even when the suite actually does not have
         one. This typically does not matter, but with bigger suite structures
-        containing a huge about of suites it can have some effect on memory usage.
+        it can have some effect on memory usage.
 
         New in Robot Framework 5.0.
         """
-
         return bool(self._setup)
 
     @property
-    def teardown(self):
-        """Suite teardown as a :class:`~.model.keyword.Keyword` object.
+    def teardown(self) -> Keyword:
+        """Suite teardown.
 
         See :attr:`setup` for more information.
         """
-        if self._teardown is None and self:
+        if self._teardown is None:
             self._teardown = create_fixture(None, self, Keyword.TEARDOWN)
         return self._teardown
 
     @teardown.setter
-    def teardown(self, teardown):
+    def teardown(self, teardown: 'Keyword|Mapping|None'):
         self._teardown = create_fixture(teardown, self, Keyword.TEARDOWN)
 
     @property
-    def has_teardown(self):
+    def has_teardown(self) -> bool:
         """Check does a suite have a teardown without creating a teardown object.
 
         See :attr:`has_setup` for more information.
 
         New in Robot Framework 5.0.
         """
         return bool(self._teardown)
 
     @property
-    def keywords(self):
-        """Deprecated since Robot Framework 4.0
+    def keywords(self) -> Keywords:
+        """Deprecated since Robot Framework 4.0.
 
         Use :attr:`setup` or :attr:`teardown` instead.
         """
         keywords = [self.setup, self.teardown]
         return Keywords(self, [kw for kw in keywords if kw])
 
     @keywords.setter
     def keywords(self, keywords):
         Keywords.raise_deprecation_error()
 
     @property
-    def id(self):
+    def id(self) -> str:
         """An automatically generated unique id.
 
         The root suite has id ``s1``, its child suites have ids ``s1-s1``,
         ``s1-s2``, ..., their child suites get ids ``s1-s1-s1``, ``s1-s1-s2``,
         ..., ``s1-s2-s1``, ..., and so on.
 
         The first test in a suite has an id like ``s1-t1``, the second has an
         id ``s1-t2``, and so on. Similarly, keywords in suites (setup/teardown)
         and in tests get ids like ``s1-k1``, ``s1-t1-k1``, and ``s1-s4-t2-k5``.
         """
         if not self.parent:
             return 's1'
-        index = self.parent.suites.index(self)
+        suites = self.parent.suites
+        index = suites.index(self) if self in suites else len(suites)
         return f'{self.parent.id}-s{index + 1}'
 
     @property
-    def all_tests(self):
+    def all_tests(self) -> Iterator[TestCase]:
         """Yields all tests this suite and its child suites contain.
 
         New in Robot Framework 6.1.
         """
         yield from self.tests
         for suite in self.suites:
             yield from suite.all_tests
 
     @property
-    def test_count(self):
+    def test_count(self) -> int:
         """Total number of the tests in this suite and in its child suites."""
         # This is considerably faster than `return len(list(self.all_tests))`.
         return len(self.tests) + sum(suite.test_count for suite in self.suites)
 
     @property
-    def has_tests(self):
+    def has_tests(self) -> bool:
         if self.tests:
             return True
         return any(s.has_tests for s in self.suites)
 
-    def set_tags(self, add=None, remove=None, persist=False):
+    def set_tags(self, add: Sequence[str] = (), remove: Sequence[str] = (),
+                 persist: bool = False):
         """Add and/or remove specified tags to the tests in this suite.
 
         :param add: Tags to add as a list or, if adding only one,
             as a single string.
         :param remove: Tags to remove as a list or as a single string.
             Can be given as patterns where ``*`` and ``?`` work as wildcards.
         :param persist: Add/remove specified tags also to new tests added
             to this suite in the future.
         """
         setter = TagSetter(add, remove)
         self.visit(setter)
         if persist:
             self._my_visitors.append(setter)
 
-    def filter(self, included_suites=None, included_tests=None,
-               included_tags=None, excluded_tags=None):
+    def filter(self, included_suites: 'Sequence[str]|None' = None,
+               included_tests: 'Sequence[str]|None' = None,
+               included_tags: 'Sequence[str]|None' = None,
+               excluded_tags: 'Sequence[str]|None' = None):
         """Select test cases and remove others from this suite.
 
         Parameters have the same semantics as ``--suite``, ``--test``,
         ``--include``, and ``--exclude`` command line options. All of them
         can be given as a list of strings, or when selecting only one, as
         a single string.
 
@@ -286,27 +292,27 @@
         """
         if self.parent is not None:
             raise ValueError("'TestSuite.configure()' can only be used with "
                              "the root test suite.")
         if options:
             self.visit(SuiteConfigurer(**options))
 
-    def remove_empty_suites(self, preserve_direct_children=False):
+    def remove_empty_suites(self, preserve_direct_children: bool = False):
         """Removes all child suites not containing any tests, recursively."""
         self.visit(EmptySuiteRemover(preserve_direct_children))
 
-    def visit(self, visitor):
+    def visit(self, visitor: SuiteVisitor):
         """:mod:`Visitor interface <robot.model.visitor>` entry-point."""
         visitor.visit_suite(self)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
-    def to_dict(self):
-        data = {'name': self.name}
+    def to_dict(self) -> 'dict[str, Any]':
+        data: 'dict[str, Any]' = {'name': self.name}
         if self.doc:
             data['doc'] = self.doc
         if self.metadata:
             data['metadata'] = dict(self.metadata)
         if self.source:
             data['source'] = str(self.source)
         if self.rpa:
@@ -318,12 +324,14 @@
         if self.tests:
             data['tests'] = self.tests.to_dicts()
         if self.suites:
             data['suites'] = self.suites.to_dicts()
         return data
 
 
-class TestSuites(ItemList):
+class TestSuites(ItemList[TestSuite]):
     __slots__ = []
 
-    def __init__(self, suite_class=TestSuite, parent=None, suites=None):
+    def __init__(self, suite_class: Type[TestSuite] = TestSuite,
+                 parent: 'TestSuite|None' = None,
+                 suites: 'Sequence[TestSuite|Mapping]' = ()):
         super().__init__(suite_class, {'parent': parent}, suites)
```

## Comparing `robotframework-6.1a1/src/robot/model/control.py` & `robotframework-6.1b1/src/robot/model/control.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,20 +85,23 @@
 
 
 @Body.register
 class While(BodyItem):
     """Represents ``WHILE`` loops."""
     type = BodyItem.WHILE
     body_class = Body
-    repr_args = ('condition', 'limit')
-    __slots__ = ['condition', 'limit']
+    repr_args = ('condition', 'limit', 'on_limit', 'on_limit_message')
+    __slots__ = ['condition', 'limit', 'on_limit', 'on_limit_message']
 
-    def __init__(self, condition=None, limit=None, parent=None):
+    def __init__(self, condition=None, limit=None, on_limit=None,
+                 on_limit_message=None, parent=None):
         self.condition = condition
+        self.on_limit = on_limit
         self.limit = limit
+        self.on_limit_message = on_limit_message
         self.parent = parent
         self.body = None
 
     @setter
     def body(self, body):
         return self.body_class(self, body)
 
@@ -107,25 +110,31 @@
 
     def __str__(self):
         parts = ['WHILE']
         if self.condition is not None:
             parts.append(self.condition)
         if self.limit is not None:
             parts.append(f'limit={self.limit}')
+        if self.on_limit is not None:
+            parts.append(f'limit={self.on_limit}')
+        if self.on_limit_message is not None:
+            parts.append(f'on_limit_message={self.on_limit_message}')
         return '    '.join(parts)
 
     def _include_in_repr(self, name, value):
         return name == 'condition' or value is not None
 
     def to_dict(self):
         data = {'type': self.type}
         if self.condition:
             data['condition'] = self.condition
         if self.limit:
             data['limit'] = self.limit
+        if self.on_limit_message:
+            data['on_limit_message'] = self.on_limit_message
         data['body'] = self.body.to_dicts()
         return data
 
 
 class IfBranch(BodyItem):
     """Represents individual ``IF``, ``ELSE IF`` or ``ELSE`` branch."""
     body_class = Body
@@ -144,15 +153,15 @@
 
     @property
     def id(self):
         """Branch id omits IF/ELSE root from the parent id part."""
         if not self.parent:
             return 'k1'
         if not self.parent.parent:
-            return 'k%d' % (self.parent.body.index(self) + 1)
+            return self._get_id(self.parent)
         return self._get_id(self.parent.parent)
 
     def __str__(self):
         if self.type == self.IF:
             return 'IF    %s' % self.condition
         if self.type == self.ELSE_IF:
             return 'ELSE IF    %s' % self.condition
@@ -221,15 +230,15 @@
 
     @property
     def id(self):
         """Branch id omits TRY/EXCEPT root from the parent id part."""
         if not self.parent:
             return 'k1'
         if not self.parent.parent:
-            return 'k%d' % (self.parent.body.index(self) + 1)
+            return self._get_id(self.parent)
         return self._get_id(self.parent.parent)
 
     def __str__(self):
         if self.type != BodyItem.EXCEPT:
             return self.type
         parts = ['EXCEPT', *self.patterns]
         if self.pattern_type:
```

## Comparing `robotframework-6.1a1/src/robot/model/metadata.py` & `robotframework-6.1b1/src/robot/model/metadata.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/suitestatistics.py` & `robotframework-6.1b1/src/robot/model/suitestatistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/modifier.py` & `robotframework-6.1b1/src/robot/model/modifier.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/keyword.py` & `robotframework-6.1b1/src/robot/model/keyword.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,144 +9,153 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from typing import Any, Sequence, Type, TYPE_CHECKING
 import warnings
 
 from .body import Body, BodyItem
 from .itemlist import ItemList
 
+if TYPE_CHECKING:
+    from .testcase import TestCase
+    from .testsuite import TestSuite
+    from .visitor import SuiteVisitor
+
 
 @Body.register
 class Keyword(BodyItem):
     """Base model for a single keyword.
 
     Extended by :class:`robot.running.model.Keyword` and
     :class:`robot.result.model.Keyword`.
     """
     repr_args = ('name', 'args', 'assign')
     __slots__ = ['_name', 'args', 'assign', 'type']
 
-    def __init__(self, name='', args=(), assign=(), type=BodyItem.KEYWORD, parent=None):
+    def __init__(self, name: str = '', args: Sequence[str] = (),
+                 assign: Sequence[str] = (), type: str = BodyItem.KEYWORD,
+                 parent: 'TestSuite|TestCase|BodyItem|None' = None):
         self._name = name
         self.args = args
         self.assign = assign
         self.type = type
         self.parent = parent
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._name
 
     @name.setter
-    def name(self, name):
+    def name(self, name: str):
         self._name = name
 
-    def visit(self, visitor):
+    def visit(self, visitor: 'SuiteVisitor'):
         """:mod:`Visitor interface <robot.model.visitor>` entry-point."""
         if self:
             visitor.visit_keyword(self)
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return self.name is not None
 
-    def __str__(self):
+    def __str__(self) -> str:
         parts = list(self.assign) + [self.name] + list(self.args)
         return '    '.join(str(p) for p in parts)
 
-    def to_dict(self):
-        data = {'name': self.name}
+    def to_dict(self) -> 'dict[str, Any]':
+        data: 'dict[str, Any]' = {'name': self.name}
         if self.args:
             data['args'] = list(self.args)
         if self.assign:
             data['assign'] = list(self.assign)
         return data
 
 
-class Keywords(ItemList):
+class Keywords(ItemList[Keyword]):
     """A list-like object representing keywords in a suite, a test or a keyword.
 
     Read-only and deprecated since Robot Framework 4.0.
     """
     __slots__ = []
     deprecation_message = (
         "'keywords' attribute is read-only and deprecated since Robot Framework 4.0. "
         "Use 'body', 'setup' or 'teardown' instead."
     )
 
-    def __init__(self, parent=None, keywords=None):
+    def __init__(self, parent: 'TestSuite|None' = None,
+                 keywords: 'Sequence[Keyword]|Keywords' = ()):
         warnings.warn(self.deprecation_message, UserWarning)
         ItemList.__init__(self, object, {'parent': parent})
         if keywords:
             ItemList.extend(self, keywords)
 
     @property
-    def setup(self):
+    def setup(self) -> 'Keyword|None':
         return self[0] if (self and self[0].type == 'SETUP') else None
 
     @setup.setter
     def setup(self, kw):
         self.raise_deprecation_error()
 
     def create_setup(self, *args, **kwargs):
         self.raise_deprecation_error()
 
     @property
-    def teardown(self):
+    def teardown(self) -> 'Keyword|None':
         return self[-1] if (self and self[-1].type == 'TEARDOWN') else None
 
     @teardown.setter
-    def teardown(self, kw):
+    def teardown(self, kw: Keyword):
         self.raise_deprecation_error()
 
     def create_teardown(self, *args, **kwargs):
         self.raise_deprecation_error()
 
     @property
-    def all(self):
+    def all(self) -> 'Keywords':
         """Iterates over all keywords, including setup and teardown."""
         return self
 
     @property
-    def normal(self):
+    def normal(self) -> 'list[Keyword]':
         """Iterates over normal keywords, omitting setup and teardown."""
         return [kw for kw in self if kw.type not in ('SETUP', 'TEARDOWN')]
 
-    def __setitem__(self, index, item):
+    def __setitem__(self, index: int, item: Keyword):
         self.raise_deprecation_error()
 
     def create(self, *args, **kwargs):
         self.raise_deprecation_error()
 
-    def append(self, item):
+    def append(self, item: Keyword):
         self.raise_deprecation_error()
 
-    def extend(self, items):
+    def extend(self, items: Sequence[Keyword]):
         self.raise_deprecation_error()
 
-    def insert(self, index, item):
+    def insert(self, index: int, item: Keyword):
         self.raise_deprecation_error()
 
-    def pop(self, *index):
+    def pop(self, *index: int):
         self.raise_deprecation_error()
 
-    def remove(self, item):
+    def remove(self, item: Keyword):
         self.raise_deprecation_error()
 
     def clear(self):
         self.raise_deprecation_error()
 
-    def __delitem__(self, index):
+    def __delitem__(self, index: int):
         self.raise_deprecation_error()
 
     def sort(self):
         self.raise_deprecation_error()
 
     def reverse(self):
         self.raise_deprecation_error()
 
     @classmethod
-    def raise_deprecation_error(cls):
+    def raise_deprecation_error(cls: 'Type[Keywords]'):
         raise AttributeError(cls.deprecation_message)
```

## Comparing `robotframework-6.1a1/src/robot/model/namepatterns.py` & `robotframework-6.1b1/src/robot/model/namepatterns.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,36 +9,39 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from typing import Iterable, Iterator
+
 from robot.utils import MultiMatcher
 
 
-class NamePatterns:
+class NamePatterns(Iterable[str]):
 
-    def __init__(self, patterns=None):
-        self._matcher = MultiMatcher(patterns, ignore='_')
+    def __init__(self, patterns: Iterator[str] = ()):
+        self.matcher = MultiMatcher(patterns, ignore='_')
 
-    def match(self, name, longname=None):
+    def match(self, name: str, longname: 'str|None' = None) -> bool:
         return self._match(name) or longname and self._match_longname(longname)
 
     def _match(self, name):
-        return self._matcher.match(name)
+        return self.matcher.match(name)
 
     def _match_longname(self, name):
         raise NotImplementedError
 
-    def __bool__(self):
-        return bool(self._matcher)
+    def __bool__(self) -> bool:
+        return bool(self.matcher)
 
-    def __iter__(self):
-        return iter(self._matcher)
+    def __iter__(self) -> Iterator[str]:
+        for matcher in self.matcher:
+            yield matcher.pattern
 
 
 class SuiteNamePatterns(NamePatterns):
 
     def _match_longname(self, name):
         while '.' in name:
             if self._match(name):
```

## Comparing `robotframework-6.1a1/src/robot/model/tagsetter.py` & `robotframework-6.1b1/src/robot/model/tagsetter.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,36 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from typing import Sequence, TYPE_CHECKING
+
 from .visitor import SuiteVisitor
 
+if TYPE_CHECKING:
+    from .keyword import Keyword
+    from .testcase import TestCase
+    from .testsuite import TestSuite
+
 
 class TagSetter(SuiteVisitor):
 
-    def __init__(self, add=None, remove=None):
+    def __init__(self, add: 'Sequence[str]|str' = (),
+                 remove: 'Sequence[str]|str' = ()):
         self.add = add
         self.remove = remove
 
-    def start_suite(self, suite):
+    def start_suite(self, suite: 'TestSuite'):
         return bool(self)
 
-    def visit_test(self, test):
+    def visit_test(self, test: 'TestCase'):
         test.tags.add(self.add)
         test.tags.remove(self.remove)
 
-    def visit_keyword(self, keyword):
+    def visit_keyword(self, keyword: 'Keyword'):
         pass
 
     def __bool__(self):
         return bool(self.add or self.remove)
```

## Comparing `robotframework-6.1a1/src/robot/model/__init__.py` & `robotframework-6.1b1/src/robot/model/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/visitor.py` & `robotframework-6.1b1/src/robot/model/visitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,25 +100,19 @@
 
 Type hints were added in Robot Framework 6.1. They are optional and can be
 removed altogether if they get in the way.
 """
 
 from typing import TYPE_CHECKING
 
-from .body import BodyItem
-from .control import (Break, Continue, Error, For, If, IfBranch, Return, Try,
-                      TryBranch, While)
-from .keyword import Keyword
-from .message import Message
-from .testcase import TestCase
-
-# Avoid circular imports.
 if TYPE_CHECKING:
+    from robot.model import (Break, BodyItem, Continue, Error, For, If, IfBranch,
+                             Keyword, Message, Return, TestCase, TestSuite, Try,
+                             TryBranch, While)
     from robot.result import ForIteration, WhileIteration
-    from .testsuite import TestSuite
 
 
 class SuiteVisitor:
     """Abstract class to ease traversing through the suite structure.
 
     See the :mod:`module level <robot.model.visitor>` documentation for more
     information and an example.
@@ -136,100 +130,106 @@
                 suite.setup.visit(self)
             suite.suites.visit(self)
             suite.tests.visit(self)
             if suite.has_teardown:
                 suite.teardown.visit(self)
             self.end_suite(suite)
 
-    def start_suite(self, suite: 'TestSuite'):
+    def start_suite(self, suite: 'TestSuite') -> 'bool|None':
         """Called when a suite starts. Default implementation does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         pass
 
     def end_suite(self, suite: 'TestSuite'):
         """Called when a suite ends. Default implementation does nothing."""
         pass
 
-    def visit_test(self, test: TestCase):
+    def visit_test(self, test: 'TestCase'):
         """Implements traversing through tests.
 
         Can be overridden to allow modifying the passed in ``test`` without calling
         :meth:`start_test` or :meth:`end_test` nor visiting the body of the test.
         """
         if self.start_test(test) is not False:
             if test.has_setup:
                 test.setup.visit(self)
             test.body.visit(self)
             if test.has_teardown:
                 test.teardown.visit(self)
             self.end_test(test)
 
-    def start_test(self, test: TestCase):
+    def start_test(self, test: 'TestCase') -> 'bool|None':
         """Called when a test starts. Default implementation does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         pass
 
-    def end_test(self, test: TestCase):
+    def end_test(self, test: 'TestCase'):
         """Called when a test ends. Default implementation does nothing."""
         pass
 
-    def visit_keyword(self, keyword: Keyword):
+    def visit_keyword(self, keyword: 'Keyword'):
         """Implements traversing through keywords.
 
         Can be overridden to allow modifying the passed in ``kw`` without
         calling :meth:`start_keyword` or :meth:`end_keyword` nor visiting
         the body of the keyword
         """
         if self.start_keyword(keyword) is not False:
-            if hasattr(keyword, 'body'):
-                keyword.body.visit(self)
-            if getattr(keyword, 'has_teardown', False):
-                keyword.teardown.visit(self)
+            self._possible_body(keyword)
+            self._possible_teardown(keyword)
             self.end_keyword(keyword)
 
-    def start_keyword(self, keyword: Keyword):
+    def _possible_body(self, item: 'BodyItem'):
+        if hasattr(item, 'body'):
+            item.body.visit(self)    # type: ignore
+
+    def _possible_teardown(self, item: 'BodyItem'):
+        if getattr(item, 'has_teardown', False):
+            item.teardown.visit(self)    # type: ignore
+
+    def start_keyword(self, keyword: 'Keyword') -> 'bool|None':
         """Called when a keyword starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(keyword)
 
-    def end_keyword(self, keyword: Keyword):
+    def end_keyword(self, keyword: 'Keyword'):
         """Called when a keyword ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(keyword)
 
-    def visit_for(self, for_: For):
+    def visit_for(self, for_: 'For'):
         """Implements traversing through FOR loops.
 
         Can be overridden to allow modifying the passed in ``for_`` without
         calling :meth:`start_for` or :meth:`end_for` nor visiting body.
         """
         if self.start_for(for_) is not False:
             for_.body.visit(self)
             self.end_for(for_)
 
-    def start_for(self, for_: For):
+    def start_for(self, for_: 'For') -> 'bool|None':
         """Called when a FOR loop starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(for_)
 
-    def end_for(self, for_: For):
+    def end_for(self, for_: 'For'):
         """Called when a FOR loop ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(for_)
 
     def visit_for_iteration(self, iteration: 'ForIteration'):
@@ -242,15 +242,15 @@
         calling :meth:`start_for_iteration` or :meth:`end_for_iteration` nor visiting
         body.
         """
         if self.start_for_iteration(iteration) is not False:
             iteration.body.visit(self)
             self.end_for_iteration(iteration)
 
-    def start_for_iteration(self, iteration: 'ForIteration'):
+    def start_for_iteration(self, iteration: 'ForIteration') -> 'bool|None':
         """Called when a FOR loop iteration starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(iteration)
@@ -258,138 +258,138 @@
     def end_for_iteration(self, iteration: 'ForIteration'):
         """Called when a FOR loop iteration ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(iteration)
 
-    def visit_if(self, if_: If):
+    def visit_if(self, if_: 'If'):
         """Implements traversing through IF/ELSE structures.
 
         Notice that ``if_`` does not have any data directly. Actual IF/ELSE
         branches are in its ``body`` and they are visited separately using
         :meth:`visit_if_branch`.
 
         Can be overridden to allow modifying the passed in ``if_`` without
         calling :meth:`start_if` or :meth:`end_if` nor visiting branches.
         """
         if self.start_if(if_) is not False:
             if_.body.visit(self)
             self.end_if(if_)
 
-    def start_if(self, if_: If):
+    def start_if(self, if_: 'If') -> 'bool|None':
         """Called when an IF/ELSE structure starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(if_)
 
-    def end_if(self, if_: If):
+    def end_if(self, if_: 'If'):
         """Called when an IF/ELSE structure ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(if_)
 
-    def visit_if_branch(self, branch: IfBranch):
+    def visit_if_branch(self, branch: 'IfBranch'):
         """Implements traversing through single IF/ELSE branch.
 
         Can be overridden to allow modifying the passed in ``branch`` without
         calling :meth:`start_if_branch` or :meth:`end_if_branch` nor visiting body.
         """
         if self.start_if_branch(branch) is not False:
             branch.body.visit(self)
             self.end_if_branch(branch)
 
-    def start_if_branch(self, branch: IfBranch):
+    def start_if_branch(self, branch: 'IfBranch') -> 'bool|None':
         """Called when an IF/ELSE branch starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(branch)
 
-    def end_if_branch(self, branch: IfBranch):
+    def end_if_branch(self, branch: 'IfBranch'):
         """Called when an IF/ELSE branch ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(branch)
 
-    def visit_try(self, try_: Try):
+    def visit_try(self, try_: 'Try'):
         """Implements traversing through TRY/EXCEPT structures.
 
         This method is used with the TRY/EXCEPT root element. Actual TRY, EXCEPT, ELSE
         and FINALLY branches are visited separately using :meth:`visit_try_branch`.
         """
         if self.start_try(try_) is not False:
             try_.body.visit(self)
             self.end_try(try_)
 
-    def start_try(self, try_: Try):
+    def start_try(self, try_: 'Try') -> 'bool|None':
         """Called when a TRY/EXCEPT structure starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(try_)
 
-    def end_try(self, try_: Try):
+    def end_try(self, try_: 'Try'):
         """Called when a TRY/EXCEPT structure ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(try_)
 
-    def visit_try_branch(self, branch: TryBranch):
+    def visit_try_branch(self, branch: 'TryBranch'):
         """Visits individual TRY, EXCEPT, ELSE and FINALLY branches."""
         if self.start_try_branch(branch) is not False:
             branch.body.visit(self)
             self.end_try_branch(branch)
 
-    def start_try_branch(self, branch: TryBranch):
+    def start_try_branch(self, branch: 'TryBranch') -> 'bool|None':
         """Called when TRY, EXCEPT, ELSE or FINALLY branches start.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(branch)
 
-    def end_try_branch(self, branch: TryBranch):
+    def end_try_branch(self, branch: 'TryBranch'):
         """Called when TRY, EXCEPT, ELSE and FINALLY branches end.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(branch)
 
-    def visit_while(self, while_: While):
+    def visit_while(self, while_: 'While'):
         """Implements traversing through WHILE loops.
 
         Can be overridden to allow modifying the passed in ``while_`` without
         calling :meth:`start_while` or :meth:`end_while` nor visiting body.
         """
         if self.start_while(while_) is not False:
             while_.body.visit(self)
             self.end_while(while_)
 
-    def start_while(self, while_: While):
+    def start_while(self, while_: 'While') -> 'bool|None':
         """Called when a WHILE loop starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(while_)
 
-    def end_while(self, while_: While):
+    def end_while(self, while_: 'While'):
         """Called when a WHILE loop ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(while_)
 
     def visit_while_iteration(self, iteration: 'WhileIteration'):
@@ -402,15 +402,15 @@
         calling :meth:`start_while_iteration` or :meth:`end_while_iteration` nor visiting
         body.
         """
         if self.start_while_iteration(iteration) is not False:
             iteration.body.visit(self)
             self.end_while_iteration(iteration)
 
-    def start_while_iteration(self, iteration: 'WhileIteration'):
+    def start_while_iteration(self, iteration: 'WhileIteration') -> 'bool|None':
         """Called when a WHILE loop iteration starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(iteration)
@@ -418,148 +418,144 @@
     def end_while_iteration(self, iteration: 'WhileIteration'):
         """Called when a WHILE loop iteration ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(iteration)
 
-    def visit_return(self, return_: Return):
+    def visit_return(self, return_: 'Return'):
         """Visits a RETURN elements."""
         if self.start_return(return_) is not False:
-            if hasattr(return_, 'body'):
-                return_.body.visit(self)
+            self._possible_body(return_)
             self.end_return(return_)
 
-    def start_return(self, return_: Return):
+    def start_return(self, return_: 'Return') -> 'bool|None':
         """Called when a RETURN element starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(return_)
 
-    def end_return(self, return_: Return):
+    def end_return(self, return_: 'Return'):
         """Called when a RETURN element ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(return_)
 
-    def visit_continue(self, continue_: Continue):
+    def visit_continue(self, continue_: 'Continue'):
         """Visits CONTINUE elements."""
         if self.start_continue(continue_) is not False:
-            if hasattr(continue_, 'body'):
-                continue_.body.visit(self)
+            self._possible_body(continue_)
             self.end_continue(continue_)
 
-    def start_continue(self, continue_: Continue):
+    def start_continue(self, continue_: 'Continue') -> 'bool|None':
         """Called when a CONTINUE element starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(continue_)
 
-    def end_continue(self, continue_: Continue):
+    def end_continue(self, continue_: 'Continue'):
         """Called when a CONTINUE element ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(continue_)
 
-    def visit_break(self, break_: Break):
+    def visit_break(self, break_: 'Break'):
         """Visits BREAK elements."""
         if self.start_break(break_) is not False:
-            if hasattr(break_, 'body'):
-                break_.body.visit(self)
+            self._possible_body(break_)
             self.end_break(break_)
 
-    def start_break(self, break_: Break):
+    def start_break(self, break_: 'Break') -> 'bool|None':
         """Called when a BREAK element starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(break_)
 
-    def end_break(self, break_: Break):
+    def end_break(self, break_: 'Break'):
         """Called when a BREAK element ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(break_)
 
-    def visit_error(self, error: Error):
+    def visit_error(self, error: 'Error'):
         """Visits body items resulting from invalid syntax.
 
         Examples include syntax like ``END`` or ``ELSE`` in wrong place and
         invalid setting like ``[Invalid]``.
         """
         if self.start_error(error) is not False:
-            if hasattr(error, 'body'):
-                error.body.visit(self)
+            self._possible_body(error)
             self.end_error(error)
 
-    def start_error(self, error: Error):
+    def start_error(self, error: 'Error') -> 'bool|None':
         """Called when a ERROR element starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(error)
 
-    def end_error(self, error: Error):
+    def end_error(self, error: 'Error'):
         """Called when a ERROR element ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(error)
 
-    def visit_message(self, message: Message):
+    def visit_message(self, message: 'Message'):
         """Implements visiting messages.
 
         Can be overridden to allow modifying the passed in ``msg`` without
         calling :meth:`start_message` or :meth:`end_message`.
         """
         if self.start_message(message) is not False:
             self.end_message(message)
 
-    def start_message(self, message: Message):
+    def start_message(self, message: 'Message') -> 'bool|None':
         """Called when a message starts.
 
         By default, calls :meth:`start_body_item` which, by default, does nothing.
 
         Can return explicit ``False`` to stop visiting.
         """
         return self.start_body_item(message)
 
-    def end_message(self, message: Message):
+    def end_message(self, message: 'Message'):
         """Called when a message ends.
 
         By default, calls :meth:`end_body_item` which, by default, does nothing.
         """
         self.end_body_item(message)
 
-    def start_body_item(self, item: BodyItem):
+    def start_body_item(self, item: 'BodyItem') -> 'bool|None':
         """Called, by default, when keywords, messages or control structures start.
 
         More specific :meth:`start_keyword`, :meth:`start_message`, `:meth:`start_for`,
         etc. can be implemented to visit only keywords, messages or specific control
         structures.
 
         Can return explicit ``False`` to stop visiting. Default implementation does
         nothing.
         """
         pass
 
-    def end_body_item(self, item: BodyItem):
+    def end_body_item(self, item: 'BodyItem'):
         """Called, by default, when keywords, messages or control structures end.
 
         More specific :meth:`end_keyword`, :meth:`end_message`, `:meth:`end_for`,
         etc. can be implemented to visit only keywords, messages or specific control
         structures.
 
         Default implementation does nothing.
```

## Comparing `robotframework-6.1a1/src/robot/model/totalstatistics.py` & `robotframework-6.1b1/src/robot/model/totalstatistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/filter.py` & `robotframework-6.1b1/src/robot/model/filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,102 +9,100 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from typing import Sequence, TYPE_CHECKING
+
 from robot.utils import setter
 
 from .tags import TagPatterns
 from .namepatterns import SuiteNamePatterns, TestNamePatterns
 from .visitor import SuiteVisitor
 
+if TYPE_CHECKING:
+    from .keyword import Keyword
+    from .testcase import TestCase
+    from .testsuite import TestSuite
+
 
 class EmptySuiteRemover(SuiteVisitor):
 
-    def __init__(self, preserve_direct_children=False):
+    def __init__(self, preserve_direct_children: bool = False):
         self.preserve_direct_children = preserve_direct_children
 
-    def end_suite(self, suite):
+    def end_suite(self, suite: 'TestSuite'):
         if suite.parent or not self.preserve_direct_children:
             suite.suites = [s for s in suite.suites if s.test_count]
 
-    def visit_test(self, test):
+    def visit_test(self, test: 'TestCase'):
         pass
 
-    def visit_keyword(self, kw):
+    def visit_keyword(self, keyword: 'Keyword'):
         pass
 
 
 class Filter(EmptySuiteRemover):
 
-    def __init__(self, include_suites=None, include_tests=None,
-                 include_tags=None, exclude_tags=None):
+    def __init__(self,
+                 include_suites: 'SuiteNamePatterns|Sequence[str]|None' = None,
+                 include_tests: 'TestNamePatterns|Sequence[str]|None' = None,
+                 include_tags: 'TagPatterns|Sequence[str]|None' = None,
+                 exclude_tags: 'TagPatterns|Sequence[str]|None' = None):
         super().__init__()
         self.include_suites = include_suites
         self.include_tests = include_tests
         self.include_tags = include_tags
         self.exclude_tags = exclude_tags
 
     @setter
-    def include_suites(self, suites):
+    def include_suites(self, suites) -> 'SuiteNamePatterns|None':
         return self._patterns_or_none(suites, SuiteNamePatterns)
 
     @setter
-    def include_tests(self, tests):
+    def include_tests(self, tests) -> 'TestNamePatterns|None':
         return self._patterns_or_none(tests, TestNamePatterns)
 
     @setter
-    def include_tags(self, tags):
+    def include_tags(self, tags) -> 'TagPatterns|None':
         return self._patterns_or_none(tags, TagPatterns)
 
     @setter
-    def exclude_tags(self, tags):
+    def exclude_tags(self, tags) -> 'TagPatterns|None':
         return self._patterns_or_none(tags, TagPatterns)
 
     def _patterns_or_none(self, items, pattern_class):
         if items is None or isinstance(items, pattern_class):
             return items
         return pattern_class(items)
 
-    def start_suite(self, suite):
+    def start_suite(self, suite: 'TestSuite'):
         if not self:
             return False
         if hasattr(suite, 'starttime'):
             suite.starttime = suite.endtime = None
         if self.include_suites is not None:
-            return self._filter_by_suite_name(suite)
+            if self.include_suites.match(suite.name, suite.longname):
+                suite.visit(Filter(include_tests=self.include_tests,
+                                   include_tags=self.include_tags,
+                                   exclude_tags=self.exclude_tags))
+                return False
+            suite.tests = []
+            return True
         if self.include_tests is not None:
-            suite.tests = self._filter(suite, self._included_by_test_name)
+            suite.tests = [t for t in suite.tests
+                           if self.include_tests.match(t.name, t.longname)]
         if self.include_tags is not None:
-            suite.tests = self._filter(suite, self._included_by_tags)
+            suite.tests = [t for t in suite.tests
+                           if self.include_tags.match(t.tags)]
         if self.exclude_tags is not None:
-            suite.tests = self._filter(suite, self._not_excluded_by_tags)
+            suite.tests = [t for t in suite.tests
+                           if not self.exclude_tags.match(t.tags)]
         return bool(suite.suites)
 
-    def _filter_by_suite_name(self, suite):
-        if self.include_suites.match(suite.name, suite.longname):
-            suite.visit(Filter(include_tests=self.include_tests,
-                               include_tags=self.include_tags,
-                               exclude_tags=self.exclude_tags))
-            return False
-        suite.tests = []
-        return True
-
-    def _filter(self, suite, filter):
-        return [t for t in suite.tests if filter(t)]
-
-    def _included_by_test_name(self, test):
-        return self.include_tests.match(test.name, test.longname)
-
-    def _included_by_tags(self, test):
-        return self.include_tags.match(test.tags)
-
-    def _not_excluded_by_tags(self, test):
-        return not self.exclude_tags.match(test.tags)
-
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self.include_suites is not None or
                     self.include_tests is not None or
                     self.include_tags is not None or
                     self.exclude_tags is not None)
```

## Comparing `robotframework-6.1a1/src/robot/model/modelobject.py` & `robotframework-6.1b1/src/robot/model/modelobject.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/configurer.py` & `robotframework-6.1b1/src/robot/model/configurer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/statistics.py` & `robotframework-6.1b1/src/robot/model/statistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/model/tagstatistics.py` & `robotframework-6.1b1/src/robot/model/tagstatistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/conf/settings.py` & `robotframework-6.1b1/src/robot/conf/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,15 @@
                  'Log'              : ('log', 'log.html'),
                  'Report'           : ('report', 'report.html'),
                  'XUnit'            : ('xunit', None),
                  'SplitLog'         : ('splitlog', False),
                  'TimestampOutputs' : ('timestampoutputs', False),
                  'LogTitle'         : ('logtitle', None),
                  'ReportTitle'      : ('reporttitle', None),
-                 'ReportBackground' : ('reportbackground',
-                                       ('#9e9', '#f66', '#fed84f')),
+                 'ReportBackground' : ('reportbackground', ('#9e9', '#f66', '#fed84f')),
                  'SuiteStatLevel'   : ('suitestatlevel', -1),
                  'TagStatInclude'   : ('tagstatinclude', []),
                  'TagStatExclude'   : ('tagstatexclude', []),
                  'TagStatCombine'   : ('tagstatcombine', []),
                  'TagDoc'           : ('tagdoc', []),
                  'TagStatLink'      : ('tagstatlink', []),
                  'RemoveKeywords'   : ('removekeywords', []),
@@ -466,14 +465,15 @@
                        'SkipTeardownOnExit' : ('skipteardownonexit', False),
                        'ReRunFailed'        : ('rerunfailed', None),
                        'ReRunFailedSuites'  : ('rerunfailedsuites', None),
                        'Randomize'          : ('randomize', 'NONE'),
                        'RunEmptySuite'      : ('runemptysuite', False),
                        'Variables'          : ('variable', []),
                        'VariableFiles'      : ('variablefile', []),
+                       'Parsers'            : ('parser', []),
                        'PreRunModifiers'    : ('prerunmodifier', []),
                        'Listeners'          : ('listener', []),
                        'ConsoleType'        : ('console', 'verbose'),
                        'ConsoleTypeDotted'  : ('dotted', False),
                        'ConsoleTypeQuiet'   : ('quiet', False),
                        'ConsoleWidth'       : ('consolewidth', 78),
                        'ConsoleMarkers'     : ('consolemarkers', 'AUTO'),
@@ -626,14 +626,18 @@
         return self['MaxErrorLines']
 
     @property
     def max_assign_length(self):
         return self['MaxAssignLength']
 
     @property
+    def parsers(self):
+        return self['Parsers']
+
+    @property
     def pre_run_modifiers(self):
         return self['PreRunModifiers']
 
     @property
     def run_empty_suite(self):
         return self['RunEmptySuite']
```

## Comparing `robotframework-6.1a1/src/robot/conf/__init__.py` & `robotframework-6.1b1/src/robot/conf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 the framework. There should be no need to use these classes externally.
 
 This package can be considered relatively stable. Aforementioned classes
 are likely to be rewritten at some point to be more convenient to use.
 Instantiating them is not likely to change, though.
 """
 
-from .languages import Languages, Language
+from .languages import Language, LanguageLike, Languages, LanguagesLike
 from .settings import RobotSettings, RebotSettings
```

## Comparing `robotframework-6.1a1/src/robot/conf/languages.py` & `robotframework-6.1b1/src/robot/conf/languages.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,102 +11,118 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import inspect
 from itertools import chain
-import os.path
+from pathlib import Path
+from typing import cast, Iterable, Iterator, Union
 
 from robot.errors import DataError
 from robot.utils import classproperty, is_list_like, Importer, normalize
 
 
+LanguageLike = Union['Language', str, Path]
+LanguagesLike = Union['Languages', LanguageLike, Iterable[LanguageLike], None]
+
+
 class Languages:
-    """Keeps a list of languages and unifies the translations in the properties.
+    """Stores languages and unifies translations.
 
     Example::
 
         languages = Languages('de', add_english=False)
         print(languages.settings)
         languages = Languages(['pt-BR', 'Finnish', 'MyLang.py'])
         for lang in languages:
             print(lang.name, lang.code)
     """
 
-    def __init__(self, languages=None, add_english=True):
+    def __init__(self, languages: 'Iterable[LanguageLike]|LanguageLike|None' = (),
+                 add_english: bool = True):
         """
         :param languages: Initial language or list of languages.
             Languages can be given as language codes or names, paths or names of
             language modules to load, or as :class:`Language` instances.
         :param add_english: If True, English is added automatically.
         :raises: :class:`~robot.errors.DataError` if a given language is not found.
 
         :meth:`add_language` can be used to add languages after initialization.
         """
-        self.languages = []
-        self.headers = {}
-        self.settings = {}
-        self.bdd_prefixes = set()
-        self.true_strings = {'True', '1'}
-        self.false_strings = {'False', '0', 'None', ''}
+        self.languages: 'list[Language]' = []
+        self.headers: 'dict[str, str]' = {}
+        self.settings: 'dict[str, str]' = {}
+        self.bdd_prefixes:  'set[str]' = set()
+        self.true_strings: 'set[str]' = {'True', '1'}
+        self.false_strings: 'set[str]' = {'False', '0', 'None', ''}
         for lang in self._get_languages(languages, add_english):
             self._add_language(lang)
 
-    def reset(self, languages=None, add_english=True):
+    def reset(self, languages: Iterable[LanguageLike] = (), add_english: bool = True):
         """Resets the instance to the given languages."""
         self.__init__(languages, add_english)
 
-    def add_language(self, lang):
+    def add_language(self, lang: LanguageLike):
         """Add new language.
 
         :param lang: Language to add. Can be a language code or name, name or
             path of a language module to load, or a :class:`Language` instance.
         :raises: :class:`~robot.errors.DataError` if the language is not found.
 
         Language codes and names are passed to by :meth:`Language.from_name`.
         Language modules are imported and :class:`Language` subclasses in them
         loaded.
         """
-        try:
-            if isinstance(lang, Language):
-                languages = [lang]
-            else:
-                languages = [Language.from_name(lang)]
-        except ValueError as err1:
+        if isinstance(lang, Language):
+            languages = [lang]
+        elif isinstance(lang, Path) or self._exists(Path(lang)):
+            languages = self._import_language_module(Path(lang))
+        else:
             try:
-                languages = self._import_languages(lang)
-            except DataError as err2:
-                raise DataError(f'{err1} {err2}')
+                languages = [Language.from_name(lang)]
+            except ValueError as err1:
+                try:
+                    languages = self._import_language_module(lang)
+                except DataError as err2:
+                    raise DataError(f'{err1} {err2}') from None
         for lang in languages:
             self._add_language(lang)
 
-    def _add_language(self, lang):
+    def _exists(self, path: Path):
+        try:
+            return path.exists()
+        except OSError:    # Can happen on Windows w/ Python < 3.10.
+            return False
+
+    def _add_language(self, lang: 'Language'):
         if lang in self.languages:
             return
         self.languages.append(lang)
         self.headers.update({n.title(): lang.headers[n] for n in lang.headers if n})
         self.settings.update({n.title(): lang.settings[n] for n in lang.settings if n})
         self.bdd_prefixes |= {p.title() for p in lang.bdd_prefixes}
         self.true_strings |= {s.title() for s in lang.true_strings}
         self.false_strings |= {s.title() for s in lang.false_strings}
 
-    def _get_languages(self, languages, add_english=True):
+    def _get_languages(self, languages, add_english=True) -> 'list[Language]':
         languages = self._resolve_languages(languages, add_english)
         available = self._get_available_languages()
-        returned = []
+        returned: 'list[Language]' = []
         for lang in languages:
             if isinstance(lang, Language):
                 returned.append(lang)
+            elif isinstance(lang, Path):
+                returned.extend(self._import_language_module(lang))
             else:
                 normalized = normalize(lang, ignore='-')
                 if normalized in available:
                     returned.append(available[normalized]())
                 else:
-                    returned.extend(self._import_languages(lang))
+                    returned.extend(self._import_language_module(lang))
         return returned
 
     def _resolve_languages(self, languages, add_english=True):
         if not languages:
             languages = []
         elif is_list_like(languages):
             languages = list(languages)
@@ -121,34 +137,36 @@
                 'Test Case': 'Test Cases',
                 'Task': 'Tasks',
                 'Keyword': 'Keywords',
                 'Comment': 'Comments'
             }
         return languages
 
-    def _get_available_languages(self):
+    def _get_available_languages(self) -> 'dict[str, type[Language]]':
         available = {}
         for lang in Language.__subclasses__():
-            available[normalize(lang.code, ignore='-')] = lang
-            available[normalize(lang.name)] = lang
+            available[normalize(cast(str, lang.code), ignore='-')] = lang
+            available[normalize(cast(str, lang.name))] = lang
         if '' in available:
             available.pop('')
         return available
 
-    def _import_languages(self, lang):
+    def _import_language_module(self, name_or_path) -> 'list[Language]':
         def is_language(member):
             return (inspect.isclass(member)
                     and issubclass(member, Language)
                     and member is not Language)
-        if os.path.exists(lang):
-            lang = os.path.abspath(lang)
-        module = Importer('language file').import_module(lang)
+        if isinstance(name_or_path, Path):
+            name_or_path = name_or_path.absolute()
+        elif self._exists(Path(name_or_path)):
+            name_or_path = Path(name_or_path).absolute()
+        module = Importer('language file').import_module(name_or_path)
         return [value() for _, value in inspect.getmembers(module, is_language)]
 
-    def __iter__(self):
+    def __iter__(self) -> 'Iterator[Language]':
         return iter(self.languages)
 
 
 class Language:
     """Base class for language definitions.
 
     New translations can be added by extending this class and setting class
@@ -162,14 +180,15 @@
     test_cases_header = None
     tasks_header = None
     keywords_header = None
     comments_header = None
     library_setting = None
     resource_setting = None
     variables_setting = None
+    name_setting = None
     documentation_setting = None
     metadata_setting = None
     suite_setup_setting = None
     suite_teardown_setting = None
     test_setup_setting = None
     task_setup_setting = None
     test_teardown_setting = None
@@ -192,15 +211,15 @@
     then_prefixes = []
     and_prefixes = []
     but_prefixes = []
     true_strings = []
     false_strings = []
 
     @classmethod
-    def from_name(cls, name):
+    def from_name(cls, name) -> 'Language':
         """Return language class based on given `name`.
 
         Name can either be a language name (e.g. 'Finnish' or 'Brazilian Portuguese')
         or a language code (e.g. 'fi' or 'pt-BR'). Matching is case and space
         insensitive and the hyphen is ignored when matching language codes.
 
         Raises `ValueError` if no matching language is found.
@@ -210,59 +229,60 @@
             if normalized == normalize(lang.__name__):
                 return lang()
             if lang.__doc__ and normalized == normalize(lang.__doc__.splitlines()[0]):
                 return lang()
         raise ValueError(f"No language with name '{name}' found.")
 
     @classproperty
-    def code(cls):
+    def code(cls) -> str:
         """Language code like 'fi' or 'pt-BR'.
 
         Got based on the class name. If the class name is two characters (or less),
         the code is just the name in lower case. If it is longer, a hyphen is added
         and the remainder of the class name is upper-cased.
 
         This special property can be accessed also directly from the class.
         """
         if cls is Language:
             return cls.__dict__['code']
-        code = cls.__name__.lower()
+        code = cast(type, cls).__name__.lower()
         if len(code) < 3:
             return code
         return f'{code[:2]}-{code[2:].upper()}'
 
     @classproperty
-    def name(cls):
+    def name(cls) -> str:
         """Language name like 'Finnish' or 'Brazilian Portuguese'.
 
         Got from the first line of the class docstring.
 
         This special property can be accessed also directly from the class.
         """
         if cls is Language:
             return cls.__dict__['name']
         return cls.__doc__.splitlines()[0] if cls.__doc__ else ''
 
     @property
-    def headers(self):
+    def headers(self) -> 'dict[str|None, str]':
         return {
             self.settings_header: En.settings_header,
             self.variables_header: En.variables_header,
             self.test_cases_header: En.test_cases_header,
             self.tasks_header: En.tasks_header,
             self.keywords_header: En.keywords_header,
             self.comments_header: En.comments_header
         }
 
     @property
-    def settings(self):
+    def settings(self) -> 'dict[str|None, str]':
         return {
             self.library_setting: En.library_setting,
             self.resource_setting: En.resource_setting,
             self.variables_setting: En.variables_setting,
+            self.name_setting: En.name_setting,
             self.documentation_setting: En.documentation_setting,
             self.metadata_setting: En.metadata_setting,
             self.suite_setup_setting: En.suite_setup_setting,
             self.suite_teardown_setting: En.suite_teardown_setting,
             self.test_setup_setting: En.test_setup_setting,
             self.task_setup_setting: En.task_setup_setting,
             self.test_teardown_setting: En.test_teardown_setting,
@@ -279,15 +299,15 @@
             self.teardown_setting: En.teardown_setting,
             self.template_setting: En.template_setting,
             self.timeout_setting: En.timeout_setting,
             self.arguments_setting: En.arguments_setting,
         }
 
     @property
-    def bdd_prefixes(self):
+    def bdd_prefixes(self) -> 'set[str]':
         return set(chain(self.given_prefixes, self.when_prefixes, self.then_prefixes,
                          self.and_prefixes, self.but_prefixes))
 
     def __eq__(self, other):
         return isinstance(other, type(self))
 
     def __hash__(self):
@@ -301,14 +321,15 @@
     test_cases_header = 'Test Cases'
     tasks_header = 'Tasks'
     keywords_header = 'Keywords'
     comments_header = 'Comments'
     library_setting = 'Library'
     resource_setting = 'Resource'
     variables_setting = 'Variables'
+    name_setting = 'Name'
     documentation_setting = 'Documentation'
     metadata_setting = 'Metadata'
     suite_setup_setting = 'Suite Setup'
     suite_teardown_setting = 'Suite Teardown'
     test_setup_setting = 'Test Setup'
     task_setup_setting = 'Task Setup'
     test_teardown_setting = 'Test Teardown'
@@ -465,14 +486,15 @@
     keywords_header = 'Avainsanat'
     comments_header = 'Kommentit'
     library_setting = 'Kirjasto'
     resource_setting = 'Resurssi'
     variables_setting = 'Muuttujat'
     documentation_setting = 'Dokumentaatio'
     metadata_setting = 'Metatiedot'
+    name_setting = "Nimi"
     suite_setup_setting = 'Setin Alustus'
     suite_teardown_setting = 'Setin Alasajo'
     test_setup_setting = 'Testin Alustus'
     task_setup_setting = 'Tehtävän Alustus'
     test_teardown_setting = 'Testin Alasajo'
     task_teardown_setting = 'Tehtävän Alasajo'
     test_template_setting = 'Testin Malli'
@@ -707,14 +729,15 @@
     test_cases_header = 'Przypadki testowe'
     tasks_header = 'Zadania'
     keywords_header = 'Słowa kluczowe'
     comments_header = 'Komentarze'
     library_setting = 'Biblioteka'
     resource_setting = 'Zasób'
     variables_setting = 'Zmienne'
+    name_setting = "Nazwa"
     documentation_setting = 'Dokumentacja'
     metadata_setting = 'Metadane'
     suite_setup_setting = 'Inicjalizacja zestawu'
     suite_teardown_setting = 'Ukończenie zestawu'
     test_setup_setting = 'Inicjalizacja testu'
     test_teardown_setting = 'Ukończenie testu'
     test_template_setting = 'Szablon testu'
```

## Comparing `robotframework-6.1a1/src/robot/conf/gatherfailed.py` & `robotframework-6.1b1/src/robot/conf/gatherfailed.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/variables.py` & `robotframework-6.1b1/src/robot/variables/variables.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/scopes.py` & `robotframework-6.1b1/src/robot/variables/scopes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/store.py` & `robotframework-6.1b1/src/robot/variables/store.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/search.py` & `robotframework-6.1b1/src/robot/variables/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,31 +110,31 @@
 
     def is_list_variable(self):
         return self.identifier == '@' and self.is_variable()
 
     def is_dict_variable(self):
         return self.identifier == '&' and self.is_variable()
 
-    def is_assign(self, allow_assign_mark=False):
+    def is_assign(self, allow_assign_mark=False, allow_nested=False):
         if allow_assign_mark and self.string.endswith('='):
             match = search_variable(self.string[:-1].rstrip(), ignore_errors=True)
             return match.is_assign()
         return (self.is_variable()
                 and self.identifier in '$@&'
                 and not self.items
-                and not search_variable(self.base))
+                and (allow_nested or not search_variable(self.base)))
 
-    def is_scalar_assign(self, allow_assign_mark=False):
-        return self.identifier == '$' and self.is_assign(allow_assign_mark)
+    def is_scalar_assign(self, allow_assign_mark=False, allow_nested=False):
+        return self.identifier == '$' and self.is_assign(allow_assign_mark, allow_nested)
 
-    def is_list_assign(self, allow_assign_mark=False):
-        return self.identifier == '@' and self.is_assign(allow_assign_mark)
+    def is_list_assign(self, allow_assign_mark=False, allow_nested=False):
+        return self.identifier == '@' and self.is_assign(allow_assign_mark, allow_nested)
 
-    def is_dict_assign(self, allow_assign_mark=False):
-        return self.identifier == '&' and self.is_assign(allow_assign_mark)
+    def is_dict_assign(self, allow_assign_mark=False, allow_nested=False):
+        return self.identifier == '&' and self.is_assign(allow_assign_mark, allow_nested)
 
     def __bool__(self):
         return self.identifier is not None
 
     def __str__(self):
         if not self:
             return '<no match>'
```

## Comparing `robotframework-6.1a1/src/robot/variables/replacer.py` & `robotframework-6.1b1/src/robot/variables/replacer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/assigner.py` & `robotframework-6.1b1/src/robot/variables/assigner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/notfound.py` & `robotframework-6.1b1/src/robot/variables/notfound.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/finders.py` & `robotframework-6.1b1/src/robot/variables/finders.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/__init__.py` & `robotframework-6.1b1/src/robot/variables/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/filesetter.py` & `robotframework-6.1b1/src/robot/variables/filesetter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/evaluation.py` & `robotframework-6.1b1/src/robot/variables/evaluation.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/tablesetter.py` & `robotframework-6.1b1/src/robot/variables/tablesetter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/variables/resolvable.py` & `robotframework-6.1b1/src/robot/variables/resolvable.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/writer.py` & `robotframework-6.1b1/src/robot/libdocpkg/writer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/builder.py` & `robotframework-6.1b1/src/robot/libdocpkg/builder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/jsonbuilder.py` & `robotframework-6.1b1/src/robot/libdocpkg/jsonbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/htmlwriter.py` & `robotframework-6.1b1/src/robot/libdocpkg/htmlwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/output.py` & `robotframework-6.1b1/src/robot/libdocpkg/output.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/jsonwriter.py` & `robotframework-6.1b1/src/robot/libdocpkg/jsonwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/xmlwriter.py` & `robotframework-6.1b1/src/robot/libdocpkg/xmlwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/standardtypes.py` & `robotframework-6.1b1/src/robot/libdocpkg/standardtypes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/robotbuilder.py` & `robotframework-6.1b1/src/robot/libdocpkg/robotbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/consoleviewer.py` & `robotframework-6.1b1/src/robot/libdocpkg/consoleviewer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/datatypes.py` & `robotframework-6.1b1/src/robot/libdocpkg/datatypes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/__init__.py` & `robotframework-6.1b1/src/robot/libdocpkg/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/htmlutils.py` & `robotframework-6.1b1/src/robot/libdocpkg/htmlutils.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/model.py` & `robotframework-6.1b1/src/robot/libdocpkg/model.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libdocpkg/xmlbuilder.py` & `robotframework-6.1b1/src/robot/libdocpkg/xmlbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/xunitwriter.py` & `robotframework-6.1b1/src/robot/reporting/xunitwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/jsmodelbuilders.py` & `robotframework-6.1b1/src/robot/reporting/jsmodelbuilders.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/jsbuildingcontext.py` & `robotframework-6.1b1/src/robot/reporting/jsbuildingcontext.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/jswriter.py` & `robotframework-6.1b1/src/robot/reporting/jswriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/stringcache.py` & `robotframework-6.1b1/src/robot/reporting/stringcache.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/__init__.py` & `robotframework-6.1b1/src/robot/reporting/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/resultwriter.py` & `robotframework-6.1b1/src/robot/reporting/resultwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/logreportwriters.py` & `robotframework-6.1b1/src/robot/reporting/logreportwriters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/jsexecutionresult.py` & `robotframework-6.1b1/src/robot/reporting/jsexecutionresult.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/outputwriter.py` & `robotframework-6.1b1/src/robot/reporting/outputwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/reporting/expandkeywordmatcher.py` & `robotframework-6.1b1/src/robot/reporting/expandkeywordmatcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from robot.utils import MultiMatcher, is_list_like
+from collections.abc import Sequence
+
+from robot.result import Keyword
+from robot.utils import MultiMatcher
 
 
 class ExpandKeywordMatcher:
 
-    def __init__(self, expand_keywords):
-        self.matched_ids = []
+    def __init__(self, expand_keywords: 'str|Sequence[str]'):
+        self.matched_ids: 'list[str]' = []
         if not expand_keywords:
             expand_keywords = []
-        elif not is_list_like(expand_keywords):
+        elif isinstance(expand_keywords, str):
             expand_keywords = [expand_keywords]
         names = [n[5:] for n in expand_keywords if n[:5].lower() == 'name:']
         tags  = [p[4:] for p in expand_keywords if p[:4].lower() == 'tag:']
         self._match_name = MultiMatcher(names).match
         self._match_tags = MultiMatcher(tags).match_any
 
-    def match(self, kw):
-        if ((kw.passed or kw.skipped)
-                and (self._match_name(kw.name or '') or self._match_tags(kw.tags))):
+    def match(self, kw: Keyword):
+        if (self._match_name(kw.name or '')
+                or self._match_tags(kw.tags)) and not kw.not_run:
             self.matched_ids.append(kw.id)
```

## Comparing `robotframework-6.1a1/src/robot/running/context.py` & `robotframework-6.1b1/src/robot/running/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,23 +9,60 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import sys
+import inspect
+import asyncio
 from contextlib import contextmanager
 
 from robot.errors import DataError
 
 
+class Asynchronous:
+
+    def __init__(self):
+        self._loop_ref = None
+
+    @property
+    def event_loop(self):
+        if self._loop_ref is None:
+            self._loop_ref = asyncio.new_event_loop()
+        return self._loop_ref
+
+    def close_loop(self):
+        if self._loop_ref:
+            self._loop_ref.close()
+
+    def run_until_complete(self, coroutine):
+        return self.event_loop.run_until_complete(coroutine)
+
+    def is_loop_required(self, obj):
+        return inspect.iscoroutine(obj) and not self._is_loop_running()
+
+    def _is_loop_running(self):
+        # ensure 3.6 compatibility
+        if sys.version_info.minor == 6:
+            return asyncio._get_running_loop() is not None
+        try:
+            asyncio.get_running_loop()
+        except RuntimeError:
+            return False
+        else:
+            return True
+
+
 class ExecutionContexts:
 
     def __init__(self):
         self._contexts = []
+        self._asynchronous = Asynchronous()
 
     @property
     def current(self):
         return self._contexts[-1] if self._contexts else None
 
     @property
     def top(self):
@@ -35,42 +72,45 @@
         return iter(self._contexts)
 
     @property
     def namespaces(self):
         return (context.namespace for context in self)
 
     def start_suite(self, suite, namespace, output, dry_run=False):
-        ctx = _ExecutionContext(suite, namespace, output, dry_run)
+        ctx = _ExecutionContext(suite, namespace, output, dry_run, self._asynchronous)
         self._contexts.append(ctx)
         return ctx
 
     def end_suite(self):
         self._contexts.pop()
+        if not self._contexts:
+            self._asynchronous.close_loop()
 
 
 # This is ugly but currently needed e.g. by BuiltIn
 EXECUTION_CONTEXTS = ExecutionContexts()
 
 
 class _ExecutionContext:
     _started_keywords_threshold = 100
 
-    def __init__(self, suite, namespace, output, dry_run=False):
+    def __init__(self, suite, namespace, output, dry_run=False, asynchronous=None):
         self.suite = suite
         self.test = None
         self.timeouts = set()
         self.namespace = namespace
         self.output = output
         self.dry_run = dry_run
         self.in_suite_teardown = False
         self.in_test_teardown = False
         self.in_keyword_teardown = 0
         self.timeout_occurred = False
         self.steps = []
         self.user_keywords = []
+        self.asynchronous = asynchronous
 
     @contextmanager
     def suite_teardown(self):
         self.in_suite_teardown = True
         try:
             yield
         finally:
```

## Comparing `robotframework-6.1a1/src/robot/running/librarykeywordrunner.py` & `robotframework-6.1b1/src/robot/running/librarykeywordrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,18 @@
     def _run_with_output_captured_and_signal_monitor(self, runner, context):
         with OutputCapturer():
             return self._run_with_signal_monitoring(runner, context)
 
     def _run_with_signal_monitoring(self, runner, context):
         try:
             STOP_SIGNAL_MONITOR.start_running_keyword(context.in_teardown)
-            return runner()
+            runner_result = runner()
+            if context.asynchronous.is_loop_required(runner_result):
+                return context.asynchronous.run_until_complete(runner_result)
+            return runner_result
         finally:
             STOP_SIGNAL_MONITOR.stop_running_keyword()
 
     def dry_run(self, kw, context):
         assignment = VariableAssignment(kw.assign)
         result = self._get_result(kw, assignment)
         with StatusReporter(kw, result, context, run=False):
```

## Comparing `robotframework-6.1a1/src/robot/running/handlers.py` & `robotframework-6.1b1/src/robot/running/handlers.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/modelcombiner.py` & `robotframework-6.1b1/src/robot/running/modelcombiner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/libraryscopes.py` & `robotframework-6.1b1/src/robot/running/libraryscopes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/signalhandler.py` & `robotframework-6.1b1/src/robot/running/signalhandler.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/userkeywordrunner.py` & `robotframework-6.1b1/src/robot/running/userkeywordrunner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/bodyrunner.py` & `robotframework-6.1b1/src/robot/running/bodyrunner.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from robot.errors import (BreakLoop, ContinueLoop, DataError, ExecutionFailed,
                           ExecutionFailures, ExecutionPassed, ExecutionStatus)
 from robot.result import (For as ForResult, While as WhileResult, If as IfResult,
                           IfBranch as IfBranchResult, Try as TryResult,
                           TryBranch as TryBranchResult)
 from robot.output import librarylogger as logger
 from robot.utils import (cut_assign_value, frange, get_error_message, get_timestamp,
-                         is_list_like, is_number, plural_or_not as s, seq2str,
-                         split_from_equals, type_name, Matcher, timestr_to_secs)
+                         is_list_like, is_number, plural_or_not as s, secs_to_timestr,
+                         seq2str, split_from_equals, type_name, Matcher, timestr_to_secs)
 from robot.variables import is_dict_variable, evaluate_expression
 
 from .statusreporter import StatusReporter
 
 
 DEFAULT_WHILE_LIMIT = 10_000
 
@@ -371,22 +371,27 @@
         self._templated = templated
 
     def run(self, data):
         ctx = self._context
         error = None
         run = False
         limit = None
-        loop_result = WhileResult(data.condition, data.limit, starttime=get_timestamp())
+        loop_result = WhileResult(data.condition, data.limit,
+                                  data.on_limit, data.on_limit_message,
+                                  starttime=get_timestamp())
         iter_result = loop_result.body.create_iteration(starttime=get_timestamp())
         if self._run:
             if data.error:
                 error = DataError(data.error, syntax=True)
             elif not ctx.dry_run:
                 try:
-                    limit = WhileLimit.create(data.limit, ctx.variables)
+                    limit = WhileLimit.create(data.limit,
+                                              data.on_limit,
+                                              data.on_limit_message,
+                                              ctx.variables)
                     run = self._should_run(data.condition, ctx.variables)
                 except DataError as err:
                     error = err
         with StatusReporter(data, loop_result, self._context, run):
             if ctx.dry_run or not run:
                 self._run_iteration(data, iter_result, run)
                 if error:
@@ -401,14 +406,20 @@
                     if ctrl.earlier_failures:
                         errors.extend(ctrl.earlier_failures.get_errors())
                     if isinstance(ctrl, BreakLoop):
                         break
                 except ExecutionPassed as passed:
                     passed.set_earlier_failures(errors)
                     raise passed
+                except LimitExceeded as exceeded:
+                    if exceeded.on_limit_pass:
+                        self._context.info(exceeded.message)
+                    else:
+                        errors.append(exceeded)
+                    break
                 except ExecutionFailed as failed:
                     errors.extend(failed.get_errors())
                     if not failed.can_continue(ctx, self._templated):
                         break
                 iter_result = loop_result.body.create_iteration(starttime=get_timestamp())
                 if not self._should_run(data.condition, ctx.variables):
                     break
@@ -417,20 +428,22 @@
 
     def _run_iteration(self, data, result, run=True):
         runner = BodyRunner(self._context, run, self._templated)
         with StatusReporter(data, result, self._context, run):
             runner.run(data.body)
 
     def _should_run(self, condition, variables):
+        if not condition:
+            return True
         try:
             return evaluate_expression(condition, variables.current,
                                        resolve_variables=True)
         except Exception:
             msg = get_error_message()
-            raise DataError(f'Invalid WHILE condition: {msg}')
+            raise DataError(f'Invalid WHILE loop condition: {msg}')
 
 
 class IfRunner:
     _dry_run_stack = []
 
     def __init__(self, context, run=True, templated=False):
         self._context = context
@@ -527,15 +540,16 @@
             error = self._run_finally(data, run) or error
             if error:
                 raise error
 
     def _run_invalid(self, data):
         error_reported = False
         for branch in data.body:
-            result = TryBranchResult(branch.type, branch.patterns, branch.variable)
+            result = TryBranchResult(branch.type, branch.patterns, branch.pattern_type,
+                                     branch.variable)
             with StatusReporter(branch, result, self._context, run=False, suppress=True):
                 runner = BodyRunner(self._context, run=False, templated=self._templated)
                 runner.run(branch.body)
                 if not error_reported:
                     error_reported = True
                     raise DataError(data.error, syntax=True)
         raise ExecutionFailed(data.error, syntax=True)
@@ -621,68 +635,100 @@
                 return err
             else:
                 return None
 
 
 class WhileLimit:
 
+    def __init__(self, on_limit=None, on_limit_message=None):
+        self.on_limit = on_limit
+        self.on_limit_message = on_limit_message
+
     @classmethod
-    def create(cls, limit, variables):
+    def create(cls, limit, on_limit, on_limit_message, variables):
+        if on_limit_message:
+            try:
+                on_limit_message = variables.replace_string(on_limit_message)
+            except DataError as err:
+                raise DataError(f"Invalid WHILE loop 'on_limit_message': '{err}")
+        on_limit = cls.parse_on_limit(variables, on_limit)
         if not limit:
-            return IterationCountLimit(DEFAULT_WHILE_LIMIT)
+            return IterationCountLimit(DEFAULT_WHILE_LIMIT,
+                                       on_limit, on_limit_message)
         value = variables.replace_string(limit)
         if value.upper() == 'NONE':
             return NoLimit()
         try:
             count = int(value.replace(' ', ''))
         except ValueError:
             pass
         else:
             if count <= 0:
                 raise DataError(f"Invalid WHILE loop limit: Iteration count must be "
                                 f"a positive integer, got '{count}'.")
-            return IterationCountLimit(count)
+            return IterationCountLimit(count, on_limit, on_limit_message)
         try:
             secs = timestr_to_secs(value)
         except ValueError as err:
             raise DataError(f'Invalid WHILE loop limit: {err.args[0]}')
         else:
-            return DurationLimit(secs)
+            return DurationLimit(secs, on_limit, on_limit_message)
+
+    @classmethod
+    def parse_on_limit(cls, variables, on_limit):
+        if on_limit is None:
+            return None
+        try:
+            on_limit = variables.replace_string(on_limit)
+            if on_limit.upper() not in ['PASS', 'FAIL']:
+                raise DataError("Value must be 'PASS' or 'FAIL'.")
+        except DataError as err:
+            raise DataError(f"Invalid WHILE loop 'on_limit' value '{on_limit}': {err}")
+        else:
+            return on_limit.lower()
 
     def limit_exceeded(self):
-        raise ExecutionFailed(f"WHILE loop was aborted because it did not finish "
-                              f"within the limit of {self}. Use the 'limit' argument "
-                              f"to increase or remove the limit if needed.")
+        on_limit_pass = self.on_limit == 'pass'
+        if self.on_limit_message:
+            raise LimitExceeded(on_limit_pass, self.on_limit_message)
+        else:
+            raise LimitExceeded(
+                on_limit_pass,
+                f"WHILE loop was aborted because it did not finish within the limit of {self}. "
+                f"Use the 'limit' argument to increase or remove the limit if needed."
+            )
 
     def __enter__(self):
         raise NotImplementedError
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         return None
 
 
 class DurationLimit(WhileLimit):
 
-    def __init__(self, max_time):
+    def __init__(self, max_time, on_limit, on_limit_message):
+        super().__init__(on_limit, on_limit_message)
         self.max_time = max_time
         self.start_time = None
 
     def __enter__(self):
         if not self.start_time:
             self.start_time = time.time()
         if time.time() - self.start_time > self.max_time:
             self.limit_exceeded()
 
     def __str__(self):
-        return f'{self.max_time} seconds'
+        return secs_to_timestr(self.max_time)
 
 
 class IterationCountLimit(WhileLimit):
 
-    def __init__(self, max_iterations):
+    def __init__(self, max_iterations, on_limit, on_limit_message):
+        super().__init__(on_limit, on_limit_message)
         self.max_iterations = max_iterations
         self.current_iterations = 0
 
     def __enter__(self):
         if self.current_iterations >= self.max_iterations:
             self.limit_exceeded()
         self.current_iterations += 1
@@ -691,7 +737,14 @@
         return f'{self.max_iterations} iterations'
 
 
 class NoLimit(WhileLimit):
 
     def __enter__(self):
         pass
+
+
+class LimitExceeded(ExecutionFailed):
+
+    def __init__(self, on_limit_pass, message):
+        super().__init__(message)
+        self.on_limit_pass = on_limit_pass
```

## Comparing `robotframework-6.1a1/src/robot/running/usererrorhandler.py` & `robotframework-6.1b1/src/robot/running/usererrorhandler.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/suiterunner.py` & `robotframework-6.1b1/src/robot/running/suiterunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,23 @@
         self._output.start_test(ModelCombiner(test, result))
         status = TestStatus(self._suite_status, result, settings.skip_on_failure,
                             settings.rpa)
         if status.exit:
             self._add_exit_combine()
             result.tags.add('robot:exit')
         if status.passed:
+            if not test.error:
+                if not test.name:
+                    test.error = 'Test name cannot be empty.'
+                elif not test.body:
+                    test.error = 'Test cannot be empty.'
             if test.error:
-                error = test.error if not settings.rpa else test.error.replace('Test', 'Task')
-                status.test_failed(error)
+                if settings.rpa:
+                    test.error = test.error.replace('Test', 'Task')
+                status.test_failed(test.error)
             elif test.tags.robot('skip'):
                 status.test_skipped(
                     test_or_task("{Test} skipped using 'robot:skip' tag.",
                                  settings.rpa))
             elif self._skipped_tags.match(test.tags):
                 status.test_skipped(
                     test_or_task("{Test} skipped using '--skip' command line option.",
```

## Comparing `robotframework-6.1a1/src/robot/running/status.py` & `robotframework-6.1b1/src/robot/running/status.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/runkwregister.py` & `robotframework-6.1b1/src/robot/running/runkwregister.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/testlibraries.py` & `robotframework-6.1b1/src/robot/running/testlibraries.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/outputcapture.py` & `robotframework-6.1b1/src/robot/running/outputcapture.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/userkeyword.py` & `robotframework-6.1b1/src/robot/running/userkeyword.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/__init__.py` & `robotframework-6.1b1/src/robot/running/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,27 @@
 * :class:`~robot.running.builder.builders.TestSuiteBuilder` for creating
   executable test suites based on data on a file system.
   Instead of using this class directly, it is possible to use the
   :meth:`TestSuite.from_file_system <robot.running.model.TestSuite.from_file_system>`
   classmethod that uses it internally.
 
 * Classes used by :class:`~robot.running.model.TestSuite`, such as
-  :class:`~robot.running.model.TestCase` and :class:`~robot.running.model.Keyword`,
-  that are defined in the :mod:`robot.running.model` module.
+  :class:`~robot.running.model.TestCase`, :class:`~robot.running.model.Keyword`
+  and :class:`~robot.running.model.If` that are defined in the
+  :mod:`robot.running.model` module. These classes are typically only needed
+  in type hints.
+
+* :class:`~robot.running.builder.settings.TestDefaults` that is part of the
+  `external parsing API`__ and also typically needed only in type hints.
+
+__ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#parser-interface
 
 :class:`~robot.running.model.TestSuite` and
-:class:`~robot.running.builder.builders.TestSuiteBuilder` can be imported via
-the :mod:`robot.api` package. If other classes are needed directly, they can be
-imported via :mod:`robot.running`.
+:class:`~robot.running.builder.builders.TestSuiteBuilder` can be imported also via
+the :mod:`robot.api` package.
 
 .. note:: Prior to Robot Framework 6.1, only some classes in
           :mod:`robot.running.model` were exposed via :mod:`robot.running`.
 
 Examples
 --------
 
@@ -98,15 +104,15 @@
     # Report and xUnit files can be generated based on the result object.
     ResultWriter(result).write_results(report='skynet.html', log=None)
     # Generating log files requires processing the earlier generated output XML.
     ResultWriter('skynet.xml').write_results()
 """
 
 from .arguments import ArgInfo, ArgumentSpec, TypeConverter, TypeInfo
-from .builder import ResourceFileBuilder, TestSuiteBuilder
+from .builder import ResourceFileBuilder, TestDefaults, TestSuiteBuilder
 from .context import EXECUTION_CONTEXTS
 from .model import (Break, Continue, Error, For, If, IfBranch, Keyword, Return,
                     TestCase, TestSuite, Try, TryBranch, While)
 from .runkwregister import RUN_KW_REGISTER
 from .testlibraries import TestLibrary
 from .usererrorhandler import UserErrorHandler
 from .userkeyword import UserLibrary
```

## Comparing `robotframework-6.1a1/src/robot/running/randomizer.py` & `robotframework-6.1b1/src/robot/running/randomizer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/namespace.py` & `robotframework-6.1b1/src/robot/running/namespace.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/statusreporter.py` & `robotframework-6.1b1/src/robot/running/statusreporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from robot.errors import (ExecutionFailed, ExecutionStatus, DataError,
-                          HandlerExecutionFailed, KeywordError, VariableError)
+                          HandlerExecutionFailed)
 from robot.utils import ErrorDetails, get_timestamp
 
 from .modelcombiner import ModelCombiner
 
 
 class StatusReporter:
```

## Comparing `robotframework-6.1a1/src/robot/running/handlerstore.py` & `robotframework-6.1b1/src/robot/running/handlerstore.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/dynamicmethods.py` & `robotframework-6.1b1/src/robot/running/dynamicmethods.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/model.py` & `robotframework-6.1b1/src/robot/running/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,33 @@
 
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#programmatic-modification-of-results
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#listener-interface
 """
 
 import warnings
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from robot import model
 from robot.conf import RobotSettings
 from robot.errors import BreakLoop, ContinueLoop, DataError, ReturnFromKeyword
 from robot.model import BodyItem, create_fixture, Keywords, ModelObject
 from robot.output import LOGGER, Output, pyloggingconf
 from robot.result import (Break as BreakResult, Continue as ContinueResult,
                           Error as ErrorResult, Return as ReturnResult)
 from robot.utils import setter
 
 from .bodyrunner import ForRunner, IfRunner, KeywordRunner, TryRunner, WhileRunner
 from .randomizer import Randomizer
 from .statusreporter import StatusReporter
 
+if TYPE_CHECKING:
+    from robot.parsing import File
+    from .builder import TestDefaults
+
 
 class Body(model.Body):
     __slots__ = []
 
 
 @Body.register
 class Keyword(model.Keyword):
@@ -117,16 +122,17 @@
 
 
 @Body.register
 class While(model.While):
     __slots__ = ['lineno', 'error']
     body_class = Body
 
-    def __init__(self, condition=None, limit=None, parent=None, lineno=None, error=None):
-        super().__init__(condition, limit, parent)
+    def __init__(self, condition=None, limit=None, on_limit_message=None,
+                 parent=None, lineno=None, error=None):
+        super().__init__(condition, limit, on_limit_message, parent)
         self.lineno = lineno
         self.error = error
 
     @property
     def source(self):
         return self.parent.source if self.parent is not None else None
 
@@ -393,73 +399,86 @@
         super().__init__(name, doc, metadata, source, rpa)
         #: :class:`ResourceFile` instance containing imports, variables and
         #: keywords the suite owns. When data is parsed from the file system,
         #: this data comes from the same test case file that creates the suite.
         self.resource = ResourceFile(parent=self)
 
     @setter
-    def resource(self, resource):
+    def resource(self, resource: 'ResourceFile|dict') -> 'ResourceFile':
         if isinstance(resource, dict):
             resource = ResourceFile.from_dict(resource)
             resource.parent = self
         return resource
 
     @classmethod
-    def from_file_system(cls, *paths, **config):
+    def from_file_system(cls, *paths: 'Path|str', **config) -> 'TestSuite':
         """Create a :class:`TestSuite` object based on the given ``paths``.
 
-        ``paths`` are file or directory paths where to read the data from.
-
-        Internally utilizes the :class:`~.builders.TestSuiteBuilder` class
-        and ``config`` can be used to configure how it is initialized.
+        :param paths: File or directory paths where to read the data from.
+        :param config: Configuration parameters for :class:`~.builders.TestSuiteBuilder`
+            class that is used internally for building the suite.
 
-        New in Robot Framework 3.2.
+        See also :meth:`from_model` and :meth:`from_string`.
         """
         from .builder import TestSuiteBuilder
         return TestSuiteBuilder(**config).build(*paths)
 
     @classmethod
-    def from_model(cls, model, name=None):
+    def from_model(cls, model: 'File', name: 'str|None' = None, *,
+                   defaults: 'TestDefaults|None' = None) -> 'TestSuite':
         """Create a :class:`TestSuite` object based on the given ``model``.
 
+        :param model: Model to create the suite from.
+        :param name: Deprecated since Robot Framework 6.1.
+        :param defaults: Possible test specific defaults from suite
+            initialization files. New in Robot Framework 6.1.
+
         The model can be created by using the
         :func:`~robot.parsing.parser.parser.get_model` function and possibly
         modified by other tooling in the :mod:`robot.parsing` module.
 
-        The ``name`` argument is deprecated since Robot Framework 6.1. Users
-        should set the name and possible other attributes to the returned suite
-        separately. One easy way is using the :meth:`config` method like this::
+        Giving suite name is deprecated and users should set it and possible
+        other attributes to the returned suite separately. One easy way is using
+        the :meth:`config` method like this::
 
             suite = TestSuite.from_model(model).config(name='X', doc='Example')
 
-        New in Robot Framework 3.2.
+        See also :meth:`from_file_system` and :meth:`from_string`.
         """
         from .builder import RobotParser
-        suite = RobotParser().parse_model(model)
+        suite = RobotParser().parse_model(model, defaults)
         if name is not None:
-            # TODO: Change DeprecationWarning to more visible UserWarning in RF 6.2.
+            # TODO: Remove 'name' in RF 7.
             warnings.warn("'name' argument of 'TestSuite.from_model' is deprecated. "
-                          "Set the name to the returned suite separately.",
-                          DeprecationWarning)
+                          "Set the name to the returned suite separately.")
             suite.name = name
         return suite
 
     @classmethod
-    def from_string(cls, string, **config):
+    def from_string(cls, string: str, *, defaults: 'TestDefaults|None' = None,
+                    **config) -> 'TestSuite':
         """Create a :class:`TestSuite` object based on the given ``string``.
 
-        The string is internally parsed into a model by using the
-        :func:`~robot.parsing.parser.parser.get_model` function and ``config``
-        can be used to configure it. The model is then converted into a suite
-        by using :meth:`from_model`.
+        :param string: String to create the suite from.
+        :param defaults: Possible test specific defaults from suite
+            initialization files.
+        :param config: Configuration parameters for
+             :func:`~robot.parsing.parser.parser.get_model` used internally.
+
+        If suite name or other attributes need to be set, an easy way is using
+        the :meth:`config` method like this::
+
+            suite = TestSuite.from_string(string).config(name='X', doc='Example')
 
-        New in Robot Framework 6.1.
+        New in Robot Framework 6.1. See also :meth:`from_model` and
+        :meth:`from_file_system`.
         """
         from robot.parsing import get_model
-        return cls.from_model(get_model(string, data_only=True, **config))
+        model = get_model(string, data_only=True, **config)
+        return cls.from_model(model, defaults=defaults)
 
     def configure(self, randomize_suites=False, randomize_tests=False,
                   randomize_seed=None, **options):
         """A shortcut to configure a suite using one method call.
 
         Can only be used with the root test suite.
```

## Comparing `robotframework-6.1a1/src/robot/running/importer.py` & `robotframework-6.1b1/src/robot/running/importer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/timeouts/posix.py` & `robotframework-6.1b1/src/robot/running/timeouts/posix.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/timeouts/__init__.py` & `robotframework-6.1b1/src/robot/running/timeouts/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/timeouts/windows.py` & `robotframework-6.1b1/src/robot/running/timeouts/windows.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/builder/transformers.py` & `robotframework-6.1b1/src/robot/running/builder/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,62 +16,63 @@
 from ast import NodeVisitor
 
 from robot.errors import DataError
 from robot.output import LOGGER
 from robot.parsing import File, Token
 from robot.variables import VariableIterator
 
-from .settings import Defaults, TestSettings
+from .settings import FileSettings
 from ..model import ResourceFile, TestSuite
 
 
 class SettingsBuilder(NodeVisitor):
 
-    def __init__(self, suite: TestSuite, defaults: Defaults):
+    def __init__(self, suite: TestSuite, settings: FileSettings):
         self.suite = suite
-        self.defaults = defaults
+        self.settings = settings
 
     def visit_Documentation(self, node):
         self.suite.doc = node.value
 
     def visit_Metadata(self, node):
         self.suite.metadata[node.name] = node.value
 
+    def visit_SuiteName(self, node):
+        self.suite.name = node.value
+
     def visit_SuiteSetup(self, node):
         self.suite.setup.config(name=node.name, args=node.args,
                                 lineno=node.lineno)
 
     def visit_SuiteTeardown(self, node):
         self.suite.teardown.config(name=node.name, args=node.args,
                                    lineno=node.lineno)
 
     def visit_TestSetup(self, node):
-        self.defaults.setup = {
-            'name': node.name, 'args': node.args, 'lineno': node.lineno
-        }
+        self.settings.test_setup = {'name': node.name, 'args': node.args,
+                                    'lineno': node.lineno}
 
     def visit_TestTeardown(self, node):
-        self.defaults.teardown = {
-            'name': node.name, 'args': node.args, 'lineno': node.lineno
-        }
+        self.settings.test_teardown = {'name': node.name, 'args': node.args,
+                                       'lineno': node.lineno}
 
     def visit_TestTimeout(self, node):
-        self.defaults.timeout = node.value
+        self.settings.test_timeout = node.value
 
     def visit_DefaultTags(self, node):
-        self.defaults.default_tags = node.values
+        self.settings.default_tags = node.values
 
     def visit_ForceTags(self, node):
-        self.defaults.force_tags = node.values
+        self.settings.test_tags = node.values
 
     def visit_KeywordTags(self, node):
-        self.defaults.keyword_tags = node.values
+        self.settings.keyword_tags = node.values
 
     def visit_TestTemplate(self, node):
-        self.defaults.template = node.value
+        self.settings.test_template = node.value
 
     def visit_LibraryImport(self, node):
         self.suite.resource.imports.library(node.name, node.args, node.alias, node.lineno)
 
     def visit_ResourceImport(self, node):
         self.suite.resource.imports.resource(node.name, node.lineno)
 
@@ -86,22 +87,22 @@
 
     def visit_KeywordSection(self, node):
         pass
 
 
 class SuiteBuilder(NodeVisitor):
 
-    def __init__(self, suite: TestSuite, defaults: Defaults = None):
+    def __init__(self, suite: TestSuite, settings: FileSettings):
         self.suite = suite
-        self.defaults = defaults or Defaults()
+        self.settings = settings
         self.rpa = None
 
     def build(self, model: File):
         ErrorReporter(model.source).visit(model)
-        SettingsBuilder(self.suite, self.defaults).visit(model)
+        SettingsBuilder(self.suite, self.settings).visit(model)
         self.visit(model)
         if self.rpa is not None:
             self.suite.rpa = self.rpa
 
     def visit_SettingSection(self, node):
         pass
 
@@ -115,35 +116,35 @@
         if self.rpa is None:
             self.rpa = node.tasks
         elif self.rpa != node.tasks:
             raise DataError('One file cannot have both tests and tasks.')
         self.generic_visit(node)
 
     def visit_TestCase(self, node):
-        TestCaseBuilder(self.suite, self.defaults).visit(node)
+        TestCaseBuilder(self.suite, self.settings).visit(node)
 
     def visit_Keyword(self, node):
-        KeywordBuilder(self.suite.resource, self.defaults).visit(node)
+        KeywordBuilder(self.suite.resource, self.settings).visit(node)
 
 
 class ResourceBuilder(NodeVisitor):
 
     def __init__(self, resource: ResourceFile):
         self.resource = resource
-        self.defaults = Defaults()
+        self.settings = FileSettings()
 
     def build(self, model: File):
         ErrorReporter(model.source, raise_on_invalid_header=True).visit(model)
         self.visit(model)
 
     def visit_Documentation(self, node):
         self.resource.doc = node.value
 
     def visit_KeywordTags(self, node):
-        self.defaults.keyword_tags = node.values
+        self.settings.keyword_tags = node.values
 
     def visit_LibraryImport(self, node):
         self.resource.imports.library(node.name, node.args, node.alias, node.lineno)
 
     def visit_ResourceImport(self, node):
         self.resource.imports.resource(node.name, node.lineno)
 
@@ -153,42 +154,44 @@
     def visit_Variable(self, node):
         self.resource.variables.create(name=node.name,
                                        value=node.value,
                                        lineno=node.lineno,
                                        error=format_error(node.errors))
 
     def visit_Keyword(self, node):
-        KeywordBuilder(self.resource, self.defaults).visit(node)
+        KeywordBuilder(self.resource, self.settings).visit(node)
 
 
 class TestCaseBuilder(NodeVisitor):
 
-    def __init__(self, suite: TestSuite, defaults: Defaults):
+    def __init__(self, suite: TestSuite, settings: FileSettings):
         self.suite = suite
-        self.settings = TestSettings(defaults)
+        self.settings = settings
         self.test = None
+        self.tags = None
 
     def visit_TestCase(self, node):
-        self.test = self.suite.tests.create(name=node.name, lineno=node.lineno,
-                                            error=format_error(node.errors + node.header.errors))
+        error = format_error(node.errors + node.header.errors)
+        settings = self.settings
+        self.test = self.suite.tests.create(name=node.name,
+                                            lineno=node.lineno,
+                                            tags=settings.test_tags,
+                                            timeout=settings.test_timeout,
+                                            template=settings.test_template,
+                                            error=error)
+        if settings.test_setup:
+            self.test.setup.config(**settings.test_setup)
+        if settings.test_teardown:
+            self.test.teardown.config(**settings.test_teardown)
         self.generic_visit(node)
-        self._set_settings(self.test, self.settings)
-
-    def _set_settings(self, test, settings):
-        if settings.setup:
-            test.setup.config(**settings.setup)
-        if settings.teardown:
-            test.teardown.config(**settings.teardown)
-        if settings.timeout:
-            test.timeout = settings.timeout
-        if settings.tags:
-            test.tags = settings.tags
-        if settings.template:
-            test.template = settings.template
-            self._set_template(test, settings.template)
+        tags = self.tags if self.tags is not None else settings.default_tags
+        if tags:
+            self.test.tags.add(tags)
+        if self.test.template:
+            self._set_template(self.test, self.test.template)
 
     def _set_template(self, parent, template):
         for item in parent.body:
             if item.type == item.FOR:
                 self._set_template(item, template)
             elif item.type == item.IF_ELSE_ROOT:
                 for branch in item.body:
@@ -224,32 +227,28 @@
     def visit_TemplateArguments(self, node):
         self.test.body.create_keyword(args=node.args, lineno=node.lineno)
 
     def visit_Documentation(self, node):
         self.test.doc = node.value
 
     def visit_Setup(self, node):
-        self.settings.setup = {
-            'name': node.name, 'args': node.args, 'lineno': node.lineno
-        }
+        self.test.setup.config(name=node.name, args=node.args, lineno=node.lineno)
 
     def visit_Teardown(self, node):
-        self.settings.teardown = {
-            'name': node.name, 'args': node.args, 'lineno': node.lineno
-        }
+        self.test.teardown.config(name=node.name, args=node.args, lineno=node.lineno)
 
     def visit_Timeout(self, node):
-        self.settings.timeout = node.value
+        self.test.timeout = node.value
 
     def visit_Tags(self, node):
         deprecate_tags_starting_with_hyphen(node, self.suite.source)
-        self.settings.tags = node.values
+        self.tags = node.values
 
     def visit_Template(self, node):
-        self.settings.template = node.value
+        self.test.template = node.value
 
     def visit_KeywordCall(self, node):
         self.test.body.create_keyword(name=node.keyword, args=node.args,
                                       assign=node.assign, lineno=node.lineno)
 
     def visit_ReturnStatement(self, node):
         self.test.body.create_return(node.values, lineno=node.lineno,
@@ -266,23 +265,23 @@
     def visit_Error(self, node):
         self.test.body.create_error(lineno=node.lineno,
                                     values=node.values, error=format_error(node.errors))
 
 
 class KeywordBuilder(NodeVisitor):
 
-    def __init__(self, resource: ResourceFile, defaults: Defaults):
+    def __init__(self, resource: ResourceFile, settings: FileSettings):
         self.resource = resource
-        self.defaults = defaults
+        self.settings = settings
         self.kw = None
 
     def visit_Keyword(self, node):
         error = format_error(node.errors + node.header.errors)
         self.kw = self.resource.keywords.create(name=node.name,
-                                                tags=self.defaults.keyword_tags,
+                                                tags=self.settings.keyword_tags,
                                                 lineno=node.lineno,
                                                 error=error)
         self.generic_visit(node)
 
     def visit_Documentation(self, node):
         self.kw.doc = node.value
 
@@ -544,15 +543,16 @@
     def __init__(self, parent):
         self.parent = parent
         self.model = None
 
     def build(self, node):
         error = format_error(self._get_errors(node))
         self.model = self.parent.body.create_while(
-            node.condition, node.limit, lineno=node.lineno, error=error
+            node.condition, node.limit, node.on_limit,
+            node.on_limit_message, lineno=node.lineno, error=error
         )
         for step in node.body:
             self.visit(step)
         return self.model
 
     def _get_errors(self, node):
         errors = node.header.errors + node.errors
```

## Comparing `robotframework-6.1a1/src/robot/running/builder/builders.py` & `robotframework-6.1b1/src/robot/running/builder/builders.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,30 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from itertools import chain
+from os.path import normpath
 from pathlib import Path
+from typing import cast, Sequence
 
+from robot.conf import LanguagesLike
 from robot.errors import DataError
 from robot.output import LOGGER
-from robot.parsing import SuiteStructureBuilder, SuiteStructureVisitor
-
-from .parsers import JsonParser, RobotParser, NoInitFileDirectoryParser, RestParser
-from .settings import Defaults
+from robot.parsing import (SuiteFile, SuiteDirectory, SuiteStructure,
+                           SuiteStructureBuilder, SuiteStructureVisitor)
+from robot.utils import Importer, seq2str, split_args_from_name_or_path, type_name
+
+from ..model import ResourceFile, TestSuite
+from .parsers import (CustomParser, JsonParser, NoInitFileDirectoryParser, Parser,
+                      RestParser, RobotParser)
+from .settings import TestDefaults
 
 
 class TestSuiteBuilder:
     """Builder to construct ``TestSuite`` objects based on data on the disk.
 
     The :meth:`build` method constructs executable
     :class:`~robot.running.model.TestSuite` objects based on test data files
@@ -43,152 +51,206 @@
 
     This class is part of the public API and should be imported via the
     :mod:`robot.api` package. An alternative is using the
     :meth:`TestSuite.from_file_system <robot.running.model.TestSuite.from_file_system>`
     classmethod that uses this class internally.
     """
 
-    def __init__(self, included_suites=None, included_extensions=('.robot', '.rbt'),
-                 rpa=None, lang=None, allow_empty_suite=False, process_curdir=True):
+    def __init__(self, included_suites: Sequence[str] = (),
+                 included_extensions: Sequence[str] = ('.robot', '.rbt'),
+                 custom_parsers: Sequence[str] = (),
+                 defaults: 'TestDefaults|None' = None,
+                 rpa: 'bool|None' = None, lang: LanguagesLike = None,
+                 allow_empty_suite: bool = False, process_curdir: bool = True):
         """
-        :param include_suites:
-            List of suite names to include. If ``None`` or an empty list, all
-            suites are included. Same as using `--suite` on the command line.
+        :param included_suites:
+            List of suite names to include. If not given, all suites are included.
+            Same as using ``--suite`` on the command line.
         :param included_extensions:
-            List of extensions of files to parse. Same as `--extension`.
-        :param rpa: Explicit test execution mode. ``True`` for RPA and
-            ``False`` for test automation. By default, mode is got from data file
-            headers and possible conflicting headers cause an error.
-            Same as `--rpa` or `--norpa`.
-        :param lang: Additional languages to be supported during parsing.
+            List of extensions of files to parse. Same as ``--extension``.
+        :param custom_parsers:
+            Custom parsers as names or paths (same as ``--parser``) or as
+            parser objects. New in RF 6.1.
+        :param defaults:
+            Possible test specific defaults from suite initialization files.
+            New in RF 6.1.
+        :param rpa:
+            Explicit execution mode. ``True`` for RPA and ``False`` for test
+            automation. By default, mode is got from data file headers and possible
+            conflicting headers cause an error. Same as ``--rpa`` or ``--norpa``.
+        :param lang:
+            Additional languages to be supported during parsing.
             Can be a string matching any of the supported language codes or names,
-            an initialized :class:`~robot.conf.languages.Language` subsclass,
+            an initialized :class:`~robot.conf.languages.Language` subclass,
             a list containing such strings or instances, or a
             :class:`~robot.conf.languages.Languages` instance.
         :param allow_empty_suite:
             Specify is it an error if the built suite contains no tests.
-            Same as `--runemptysuite`.
+            Same as ``--runemptysuite``.
         :param process_curdir:
             Control processing the special ``${CURDIR}`` variable. It is
             resolved already at parsing time by default, but that can be
             changed by giving this argument ``False`` value.
         """
+        self.standard_parsers = self._get_standard_parsers(lang, process_curdir)
+        self.custom_parsers = self._get_custom_parsers(custom_parsers)
+        self.defaults = defaults
+        self.included_suites = tuple(included_suites or ())
+        self.included_extensions = tuple(included_extensions or ())
         self.rpa = rpa
-        self.lang = lang
-        self.included_suites = included_suites
-        self.included_extensions = included_extensions
         self.allow_empty_suite = allow_empty_suite
-        self.process_curdir = process_curdir
 
-    def build(self, *paths):
+    def _get_standard_parsers(self, lang: LanguagesLike,
+                              process_curdir: bool) -> 'dict[str, Parser]':
+        robot_parser = RobotParser(lang, process_curdir)
+        rest_parser = RestParser(lang, process_curdir)
+        json_parser = JsonParser()
+        return {
+            'robot': robot_parser,
+            'rst': rest_parser,
+            'rest': rest_parser,
+            'rbt': json_parser,
+            'json': json_parser
+        }
+
+    def _get_custom_parsers(self, parsers: Sequence[str]) -> 'dict[str, CustomParser]':
+        custom_parsers = {}
+        importer = Importer('parser', LOGGER)
+        for parser in parsers:
+            if isinstance(parser, (str, Path)):
+                name, args = split_args_from_name_or_path(parser)
+                parser = importer.import_class_or_module(name, args)
+            else:
+                name = type_name(parser)
+            try:
+                custom_parser = CustomParser(parser)
+            except TypeError as err:
+                raise DataError(f"Importing parser '{name}' failed: {err}")
+            for ext in custom_parser.extensions:
+                custom_parsers[ext] = custom_parser
+        return custom_parsers
+
+    def build(self, *paths: 'Path|str'):
         """
         :param paths: Paths to test data files or directories.
         :return: :class:`~robot.running.model.TestSuite` instance.
         """
-        structure = SuiteStructureBuilder(self.included_extensions,
-                                          self.included_suites).build(paths)
-        parser = SuiteStructureParser(self.included_extensions,
-                                      self.rpa, self.lang, self.process_curdir)
-        suite = parser.parse(structure)
+        paths = self._normalize_paths(paths)
+        extensions = chain(self.included_extensions, self.custom_parsers)
+        structure = SuiteStructureBuilder(extensions,
+                                          self.included_suites).build(*paths)
+        suite = SuiteStructureParser(self._get_parsers(paths), self.defaults,
+                                     self.rpa).parse(structure)
         if not self.included_suites and not self.allow_empty_suite:
-            self._validate_test_counts(suite, multisource=len(paths) > 1)
+            self._validate_not_empty(suite, multi_source=len(paths) > 1)
         suite.remove_empty_suites(preserve_direct_children=len(paths) > 1)
         return suite
 
-    def _validate_test_counts(self, suite, multisource=False):
-        def validate(suite):
-            if not suite.has_tests:
-                raise DataError(f"Suite '{suite.name}' contains no tests or tasks.")
-        if not multisource:
-            validate(suite)
-        else:
-            for s in suite.suites:
-                validate(s)
+    def _normalize_paths(self, paths: 'Sequence[Path|str]') -> 'tuple[Path, ...]':
+        if not paths:
+            raise DataError('One or more source paths required.')
+        # Cannot use `Path.resolve()` here because it resolves all symlinks which
+        # isn't desired. `Path` doesn't have any methods for normalizing paths
+        # so need to use `os.path.normpath()`. Also that _may_ resolve symlinks,
+        # but we need to do it for backwards compatibility.
+        paths = [Path(normpath(p)).absolute() for p in paths]
+        non_existing = [p for p in paths if not p.exists()]
+        if non_existing:
+            raise DataError(f"Parsing {seq2str(non_existing)} failed: "
+                            f"File or directory to execute does not exist.")
+        return tuple(paths)
+
+    def _get_parsers(self, paths: 'Sequence[Path]') -> 'dict[str|None, Parser]':
+        parsers = {None: NoInitFileDirectoryParser(), **self.custom_parsers}
+        robot_parser = self.standard_parsers['robot']
+        for ext in chain(self.included_extensions,
+                         [p.suffix for p in paths if p.is_file()]):
+            ext = ext.lstrip('.').lower()
+            if ext not in parsers:
+                parsers[ext] = self.standard_parsers.get(ext, robot_parser)
+        return parsers
+
+    def _validate_not_empty(self, suite: TestSuite, multi_source: bool = False):
+        if multi_source:
+            for child in suite.suites:
+                self._validate_not_empty(child)
+        elif not suite.has_tests:
+            raise DataError(f"Suite '{suite.name}' contains no tests or tasks.")
 
 
 class SuiteStructureParser(SuiteStructureVisitor):
 
-    def __init__(self, included_extensions, rpa=None, lang=None, process_curdir=True):
+    def __init__(self, parsers: 'dict[str|None, Parser]',
+                 defaults: 'TestDefaults|None' = None, rpa: 'bool|None' = None):
+        self.parsers = parsers
         self.rpa = rpa
+        self.defaults = defaults
         self._rpa_given = rpa is not None
-        self.suite = None
-        self._stack = []
-        self.parsers = self._get_parsers(included_extensions, lang, process_curdir)
-
-    def _get_parsers(self, extensions, lang, process_curdir):
-        robot_parser = RobotParser(lang, process_curdir)
-        rest_parser = RestParser(lang, process_curdir)
-        json_parser = JsonParser()
-        parsers = {
-            None: NoInitFileDirectoryParser(),
-            'robot': robot_parser,
-            'rst': rest_parser,
-            'rest': rest_parser,
-            'rbt': json_parser,
-            'json': json_parser
-        }
-        for ext in extensions:
-            if ext not in parsers:
-                parsers[ext] = robot_parser
-        return parsers
+        self.suite: 'TestSuite|None' = None
+        self._stack: 'list[tuple[TestSuite, TestDefaults]]' = []
 
-    def _get_parser(self, extension):
-        try:
-            return self.parsers[extension]
-        except KeyError:
-            return self.parsers['robot']
+    @property
+    def parent_defaults(self) -> 'TestDefaults|None':
+        return self._stack[-1][-1] if self._stack else self.defaults
 
-    def parse(self, structure):
+    def parse(self, structure: SuiteStructure) -> TestSuite:
         structure.visit(self)
-        self.suite.rpa = self.rpa
-        return self.suite
+        suite = cast(TestSuite, self.suite)
+        suite.rpa = self.rpa
+        return suite
 
-    def visit_file(self, structure):
+    def visit_file(self, structure: SuiteFile):
         LOGGER.info(f"Parsing file '{structure.source}'.")
-        suite, _ = self._build_suite(structure)
-        if self._stack:
-            self._stack[-1][0].suites.append(suite)
-        else:
+        suite = self._build_suite_file(structure)
+        if self.suite is None:
             self.suite = suite
+        else:
+            self._stack[-1][0].suites.append(suite)
 
-    def start_directory(self, structure):
+    def start_directory(self, structure: SuiteDirectory):
         if structure.source:
             LOGGER.info(f"Parsing directory '{structure.source}'.")
-        suite, defaults = self._build_suite(structure)
+        suite, defaults = self._build_suite_directory(structure)
         if self.suite is None:
             self.suite = suite
         else:
             self._stack[-1][0].suites.append(suite)
         self._stack.append((suite, defaults))
 
-    def end_directory(self, structure):
+    def end_directory(self, structure: SuiteDirectory):
         suite, _ = self._stack.pop()
         if suite.rpa is None and suite.suites:
             suite.rpa = suite.suites[0].rpa
 
-    def _build_suite(self, structure):
-        parent_defaults = self._stack[-1][-1] if self._stack else None
-        source = structure.source
-        defaults = Defaults(parent_defaults)
-        parser = self._get_parser(structure.extension)
+    def _build_suite_file(self, structure: SuiteFile):
+        source = cast(Path, structure.source)
+        defaults = self.parent_defaults or TestDefaults()
+        parser = self.parsers[structure.extension]
         try:
-            if structure.is_file:
-                suite = parser.parse_suite_file(source, defaults)
-                if not suite.tests:
-                    LOGGER.info(f"Data source '{source}' has no tests or tasks.")
-            else:
-                suite = parser.parse_init_file(structure.init_file or source, defaults)
-                if not source:
-                    suite.config(name='', source=None)
+            suite = parser.parse_suite_file(source, defaults)
+            if not suite.tests:
+                LOGGER.info(f"Data source '{source}' has no tests or tasks.")
             self._validate_execution_mode(suite)
         except DataError as err:
             raise DataError(f"Parsing '{source}' failed: {err.message}")
+        return suite
+
+    def _build_suite_directory(self, structure: SuiteDirectory):
+        source = cast(Path, structure.init_file or structure.source)
+        defaults = TestDefaults(self.parent_defaults)
+        parser = self.parsers[structure.extension]
+        try:
+            suite = parser.parse_init_file(source, defaults)
+            if structure.is_multi_source:
+                suite.config(name='', source=None)
+        except DataError as err:
+            raise DataError(f"Parsing '{source}' failed: {err.message}")
         return suite, defaults
 
-    def _validate_execution_mode(self, suite):
+    def _validate_execution_mode(self, suite: TestSuite):
         if self._rpa_given:
             suite.rpa = self.rpa
         elif suite.rpa is None:
             pass
         elif self.rpa is None:
             self.rpa = suite.rpa
         elif self.rpa is not suite.rpa:
@@ -197,27 +259,27 @@
                             f"but files parsed earlier have {that}. Fix headers "
                             f"or use '--rpa' or '--norpa' options to set the "
                             f"execution mode explicitly.")
 
 
 class ResourceFileBuilder:
 
-    def __init__(self, lang=None, process_curdir=True):
+    def __init__(self, lang: LanguagesLike = None, process_curdir: bool = True):
         self.lang = lang
         self.process_curdir = process_curdir
 
-    def build(self, source: Path):
+    def build(self, source: Path) -> ResourceFile:
         if not isinstance(source, Path):
             source = Path(source)
         LOGGER.info(f"Parsing resource file '{source}'.")
         resource = self._parse(source)
         if resource.imports or resource.variables or resource.keywords:
             LOGGER.info(f"Imported resource file '{source}' ({len(resource.keywords)} "
                         f"keywords).")
         else:
             LOGGER.warn(f"Imported resource file '{source}' is empty.")
         return resource
 
-    def _parse(self, source):
+    def _parse(self, source: Path) -> ResourceFile:
         if source.suffix.lower() in ('.rst', '.rest'):
             return RestParser(self.lang, self.process_curdir).parse_resource_file(source)
         return RobotParser(self.lang, self.process_curdir).parse_resource_file(source)
```

## Comparing `robotframework-6.1a1/src/robot/running/builder/__init__.py` & `robotframework-6.1b1/src/robot/running/builder/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from .builders import TestSuiteBuilder, ResourceFileBuilder
 from .parsers import RobotParser
+from .settings import TestDefaults
```

## Comparing `robotframework-6.1a1/src/robot/running/arguments/argumentmapper.py` & `robotframework-6.1b1/src/robot/running/arguments/argumentmapper.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/argumentconverter.py` & `robotframework-6.1b1/src/robot/running/arguments/argumentconverter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/argumentresolver.py` & `robotframework-6.1b1/src/robot/running/arguments/argumentresolver.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/embedded.py` & `robotframework-6.1b1/src/robot/running/arguments/embedded.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/customconverters.py` & `robotframework-6.1b1/src/robot/running/arguments/customconverters.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,38 +74,40 @@
             def converter(arg):
                 raise TypeError(f'Only {type_.__name__} instances are accepted, '
                                 f'got {type_name(arg)}.')
         if not callable(converter):
             raise TypeError(f'Custom converters must be callable, converter for '
                             f'{type_name(type_)} is {type_name(converter)}.')
         spec = cls._get_arg_spec(converter)
-        arg_type = spec.types.get(spec.positional[0])
+        arg_type = spec.types.get(spec.positional and spec.positional[0] or spec.var_positional)
         if arg_type is None:
             accepts = ()
         elif is_union(arg_type):
             accepts = arg_type.__args__
         elif hasattr(arg_type, '__origin__'):
             accepts = (arg_type.__origin__,)
         else:
             accepts = (arg_type,)
-        return cls(type_, converter, accepts, library if spec.minargs == 2 else None)
+        pass_library = spec.minargs == 2 or spec.var_positional
+        return cls(type_, converter, accepts, library if pass_library else None)
 
     @classmethod
     def _get_arg_spec(cls, converter):
         spec = PythonArgumentParser(type='Converter').parse(converter)
         if spec.minargs > 2:
             required = seq2str([a for a in spec.positional if a not in spec.defaults])
             raise TypeError(f"Custom converters cannot have more than two mandatory "
                             f"arguments, '{converter.__name__}' has {required}.")
-        if not spec.positional:
+        if not spec.maxargs:
             raise TypeError(f"Custom converters must accept one positional argument, "
                             f"'{converter.__name__}' accepts none.")
         if spec.named_only and set(spec.named_only) - set(spec.defaults):
             required = seq2str(sorted(set(spec.named_only) - set(spec.defaults)))
             raise TypeError(f"Custom converters cannot have mandatory keyword-only "
                             f"arguments, '{converter.__name__}' has {required}.")
         return spec
 
     def convert(self, value):
         if not self.library:
             return self.converter(value)
         return self.converter(value, self.library.get_instance())
+
```

## Comparing `robotframework-6.1a1/src/robot/running/arguments/typeconverters.py` & `robotframework-6.1b1/src/robot/running/arguments/typeconverters.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,19 +96,19 @@
             if not isinstance(value, str):
                 return self._non_string_convert(value, explicit_type)
             return self._convert(value, explicit_type)
         except ValueError as error:
             return self._handle_error(name, value, kind, error, strict)
 
     def no_conversion_needed(self, value):
+        used_type = getattr(self.used_type, '__origin__', self.used_type)
         try:
-            return isinstance(value, self.used_type)
+            return isinstance(value, used_type)
         except TypeError:
-            # If the used type doesn't like `isinstance` (e.g. TypedDict),
-            # compare the value to the generic type instead.
+            # Used type wasn't a class. Compare to generic type instead.
             if self.type and self.type is not self.used_type:
                 return isinstance(value, self.type)
             raise
 
     def _handles_value(self, value):
         return isinstance(value, self.value_types)
 
@@ -456,15 +456,15 @@
 
     @classmethod
     def handles(cls, type_):
         # `type_ is not Tuple` is needed with Python 3.6.
         return super().handles(type_) and type_ is not Tuple
 
     def no_conversion_needed(self, value):
-        if isinstance(value, str):
+        if isinstance(value, str) or self.converter:
             return False
         return super().no_conversion_needed(value)
 
     def _non_string_convert(self, value, explicit_type=True):
         return self._convert_items(list(value), explicit_type)
 
     def _convert(self, value, explicit_type=True):
@@ -496,14 +496,17 @@
                 raise TypeError(f'Homogenous tuple used as a type hint requires '
                                 f'exactly one nested type, got {len(types)}.')
             self.homogenous = True
         self.type_name = type_repr(used_type)
         self.converters = tuple(self.converter_for(t, custom_converters, languages)
                                 for t in types)
 
+    def no_conversion_needed(self, value):
+        return super().no_conversion_needed(value) and not self.converters
+
     def _non_string_convert(self, value, explicit_type=True):
         return self._convert_items(tuple(value), explicit_type)
 
     def _convert(self, value, explicit_type=True):
         return self._convert_items(self._literal_eval(value, tuple), explicit_type)
 
     def _convert_items(self, value, explicit_type):
@@ -583,19 +586,26 @@
         if not types:
             self.converters = ()
         else:
             self.type_name = type_repr(used_type)
             self.converters = tuple(self.converter_for(t, custom_converters, languages)
                                     for t in types)
 
+    def no_conversion_needed(self, value):
+        return super().no_conversion_needed(value) and not self.converters
+
     def _non_string_convert(self, value, explicit_type=True):
-        if issubclass(self.used_type, dict) and not isinstance(value, dict):
+        if self._used_type_is_dict() and not isinstance(value, dict):
             value = dict(value)
         return self._convert_items(value, explicit_type)
 
+    def _used_type_is_dict(self):
+        used_type = getattr(self.used_type, '__origin__', self.used_type)
+        return issubclass(used_type, dict)
+
     def _convert(self, value, explicit_type=True):
         return self._convert_items(self._literal_eval(value, dict), explicit_type)
 
     def _convert_items(self, value, explicit_type):
         if not self.converters:
             return value
         convert_key = self.__get_converter(self.converters[0], explicit_type, 'Key')
@@ -621,14 +631,17 @@
         types = self._get_nested_types(used_type, expected_count=1)
         if not types:
             self.converter = None
         else:
             self.type_name = type_repr(used_type)
             self.converter = self.converter_for(types[0], custom_converters, languages)
 
+    def no_conversion_needed(self, value):
+        return super().no_conversion_needed(value) and not self.converter
+
     def _non_string_convert(self, value, explicit_type=True):
         return self._convert_items(set(value), explicit_type)
 
     def _convert(self, value, explicit_type=True):
         return self._convert_items(self._literal_eval(value, set), explicit_type)
 
     def _convert_items(self, value, explicit_type):
```

## Comparing `robotframework-6.1a1/src/robot/running/arguments/typevalidator.py` & `robotframework-6.1b1/src/robot/running/arguments/typevalidator.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/argumentspec.py` & `robotframework-6.1b1/src/robot/running/arguments/argumentspec.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/argumentparser.py` & `robotframework-6.1b1/src/robot/running/arguments/argumentparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,19 +95,28 @@
             return getattr(handler, '__annotations__', {})
 
 
 class ArgumentSpecParser(ArgumentParser):
 
     def parse(self, argspec, name=None):
         spec = ArgumentSpec(name, self._type)
-        named_only = False
+        named_only = positional_only_separator_seen = False
         for arg in argspec:
             arg = self._validate_arg(arg)
             if spec.var_named:
                 self._report_error('Only last argument can be kwargs.')
+            elif self._is_positional_only_separator(arg):
+                if named_only:
+                    self._report_error('Positional-only separator must be before '
+                                       'named-only arguments.')
+                if positional_only_separator_seen:
+                    self._report_error('Too many positional-only separators.')
+                spec.positional_only = spec.positional_or_named
+                spec.positional_or_named = []
+                positional_only_separator_seen = True
             elif isinstance(arg, tuple):
                 arg, default = arg
                 arg = self._add_arg(spec, arg, named_only)
                 spec.defaults[arg] = default
             elif self._is_var_named(arg):
                 spec.var_named = self._format_var_named(arg)
             elif self._is_var_positional(arg):
@@ -131,14 +140,18 @@
         raise NotImplementedError
 
     @abstractmethod
     def _format_var_named(self, kwargs):
         raise NotImplementedError
 
     @abstractmethod
+    def _is_positional_only_separator(self, arg):
+        raise NotImplementedError
+
+    @abstractmethod
     def _is_named_only_separator(self, arg):
         raise NotImplementedError
 
     @abstractmethod
     def _is_var_positional(self, arg):
         raise NotImplementedError
 
@@ -179,14 +192,17 @@
 
     def _format_var_named(self, kwargs):
         return kwargs[2:]
 
     def _is_var_positional(self, arg):
         return arg and arg[0] == '*'
 
+    def _is_positional_only_separator(self, arg):
+        return arg == '/'
+
     def _is_named_only_separator(self, arg):
         return arg == '*'
 
     def _format_var_positional(self, varargs):
         return varargs[1:]
 
 
@@ -209,14 +225,17 @@
 
     def _format_var_named(self, kwargs):
         return kwargs[2:-1]
 
     def _is_var_positional(self, arg):
         return arg and arg[0] == '@'
 
+    def _is_positional_only_separator(self, arg):
+        return False
+
     def _is_named_only_separator(self, arg):
         return arg == '@{}'
 
     def _format_var_positional(self, varargs):
         return varargs[2:-1]
 
     def _format_arg(self, arg):
```

## Comparing `robotframework-6.1a1/src/robot/running/arguments/argumentvalidator.py` & `robotframework-6.1b1/src/robot/running/arguments/argumentvalidator.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/running/arguments/__init__.py` & `robotframework-6.1b1/src/robot/running/arguments/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/robotio.py` & `robotframework-6.1b1/src/robot/utils/robotio.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/filereader.py` & `robotframework-6.1b1/src/robot/utils/filereader.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,92 +9,97 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from io import StringIO
-import os.path
+from collections.abc import Iterator
+from io import IOBase, StringIO
+from pathlib import Path
+from typing import Union
 
 from .robottypes import is_bytes, is_pathlike, is_string
 
 
-class FileReader:
-    """Utility to ease reading different kind of files.
+Source = Union[Path, str, IOBase]
+
+
+class FileReader:  # FIXME: Rename to SourceReader
+    """Utility to ease reading different kind of source files.
 
     Supports different sources where to read the data:
 
     - The source can be a path to a file, either as a string or as a
-      ``pathlib.Path`` instance in Python 3. The file itself must be
-      UTF-8 encoded.
+      ``pathlib.Path`` instance. The file itself must be UTF-8 encoded.
 
     - Alternatively the source can be an already opened file object,
       including a StringIO or BytesIO object. The file can contain either
       Unicode text or UTF-8 encoded bytes.
 
     - The third options is giving the source as Unicode text directly.
       This requires setting ``accept_text=True`` when creating the reader.
 
     In all cases bytes are automatically decoded to Unicode and possible
     BOM removed.
     """
 
-    def __init__(self, source, accept_text=False):
-        self.file, self.name, self._opened = self._get_file(source, accept_text)
+    def __init__(self, source: Source, accept_text: bool = False):
+        self.file, self._opened = self._get_file(source, accept_text)
 
-    def _get_file(self, source, accept_text):
+    def _get_file(self, source: Source, accept_text: bool) -> 'tuple[IOBase, bool]':
         path = self._get_path(source, accept_text)
         if path:
             file = open(path, 'rb')
             opened = True
         elif is_string(source):
             file = StringIO(source)
             opened = True
         else:
             file = source
             opened = False
-        name = getattr(file, 'name', '<in-memory file>')
-        return file, name, opened
+        return file, opened
 
-    def _get_path(self, source, accept_text):
+    def _get_path(self, source: Source, accept_text: bool):
         if is_pathlike(source):
             return str(source)
         if not is_string(source):
             return None
         if not accept_text:
             return source
         if '\n' in source:
             return None
-        if os.path.isabs(source) or os.path.exists(source):
-            return source
-        return None
+        path = Path(source)
+        try:
+            is_path = path.is_absolute() or path.exists()
+        except OSError:    # Can happen on Windows w/ Python < 3.10.
+            is_path = False
+        return source if is_path else None
+
+    @property
+    def name(self) -> str:
+        return getattr(self.file, 'name', '<in-memory file>')
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc_info):
         if self._opened:
             self.file.close()
 
-    def read(self):
+    def read(self) -> str:
         return self._decode(self.file.read())
 
-    def readlines(self):
+    def readlines(self) -> 'Iterator[str]':
         first_line = True
         for line in self.file.readlines():
             yield self._decode(line, remove_bom=first_line)
             first_line = False
 
-    def _decode(self, content, remove_bom=True):
+    def _decode(self, content: 'str|bytes', remove_bom: bool = True) -> str:
         if is_bytes(content):
             content = content.decode('UTF-8')
         if remove_bom and content.startswith('\ufeff'):
             content = content[1:]
         if '\r\n' in content:
             content = content.replace('\r\n', '\n')
         return content
-
-    def _is_binary_file(self):
-        mode = getattr(self.file, 'mode', '')
-        encoding = getattr(self.file, 'encoding', 'ascii').lower()
-        return 'r' in mode and encoding == 'ascii'
```

## Comparing `robotframework-6.1a1/src/robot/utils/sortable.py` & `robotframework-6.1b1/src/robot/utils/sortable.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/escaping.py` & `robotframework-6.1b1/src/robot/utils/escaping.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/restreader.py` & `robotframework-6.1b1/src/robot/utils/restreader.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/frange.py` & `robotframework-6.1b1/src/robot/utils/frange.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/connectioncache.py` & `robotframework-6.1b1/src/robot/utils/connectioncache.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/normalizing.py` & `robotframework-6.1b1/src/robot/utils/normalizing.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,36 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from collections.abc import MutableMapping
 import re
+from collections.abc import Mapping, MutableMapping, Sequence
+from typing import overload
 
-from .robottypes import is_dict_like, is_string
 
+@overload
+def normalize(string: str, ignore: 'Sequence[str]' = (), caseless: bool = True,
+              spaceless: bool = True) -> str:
+    ...
+
+@overload
+def normalize(string: bytes, ignore: 'Sequence[bytes]' = (), caseless: bool = True,
+              spaceless: bool = True) -> bytes:
+    ...
 
 def normalize(string, ignore=(), caseless=True, spaceless=True):
     """Normalizes given string according to given spec.
 
     By default string is turned to lower case and all whitespace is removed.
     Additional characters can be removed by giving them in ``ignore`` list.
     """
-    empty = '' if is_string(string) else b''
+    empty = '' if isinstance(string, str) else b''
     if isinstance(ignore, bytes):
         # Iterating bytes in Python3 yields integers.
         ignore = [bytes([i]) for i in ignore]
     if spaceless:
         string = empty.join(string.split())
     if caseless:
         string = string.lower()
@@ -58,20 +67,21 @@
         Normalizing spec has exact same semantics as with the :func:`normalize`
         function.
         """
         self._data = {}
         self._keys = {}
         self._normalize = lambda s: normalize(s, ignore, caseless, spaceless)
         if initial:
-            self._add_initial(initial)
-
-    def _add_initial(self, initial):
-        items = initial.items() if hasattr(initial, 'items') else initial
-        for key, value in items:
-            self[key] = value
+            items = initial.items() if hasattr(initial, 'items') else initial
+            for key, value in items:
+                self[key] = value
+
+    @property
+    def normalized_keys(self):
+        return self._keys
 
     def __getitem__(self, key):
         return self._data[self._normalize(key)]
 
     def __setitem__(self, key, value):
         norm_key = self._normalize(key)
         self._data[norm_key] = value
@@ -85,18 +95,24 @@
     def __iter__(self):
         return (self._keys[norm_key] for norm_key in sorted(self._keys))
 
     def __len__(self):
         return len(self._data)
 
     def __str__(self):
-        return '{%s}' % ', '.join('%r: %r' % (key, self[key]) for key in self)
+        items = ', '.join(f'{key!r}: {self[key]!r}' for key in self)
+        return f'{{{items}}}'
+
+    def __repr__(self):
+        name = type(self).__name__
+        params = str(self) if self else ''
+        return f'{name}({params})'
 
     def __eq__(self, other):
-        if not is_dict_like(other):
+        if not isinstance(other, Mapping):
             return False
         if not isinstance(other, NormalizedDict):
             other = NormalizedDict(other)
         return self._data == other._data
 
     def copy(self):
         copy = NormalizedDict()
```

## Comparing `robotframework-6.1a1/src/robot/utils/markupwriters.py` & `robotframework-6.1b1/src/robot/utils/markupwriters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/compress.py` & `robotframework-6.1b1/src/robot/utils/compress.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/misc.py` & `robotframework-6.1b1/src/robot/utils/misc.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/dotdict.py` & `robotframework-6.1b1/src/robot/utils/dotdict.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/recommendations.py` & `robotframework-6.1b1/src/robot/utils/recommendations.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/text.py` & `robotframework-6.1b1/src/robot/utils/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from itertools import takewhile
 import inspect
 import os.path
 import re
+from itertools import takewhile
+from pathlib import Path
 
 from .charwidth import get_char_width
 from .misc import seq2str2
 from .robottypes import is_string
 from .unic import safe_str
 
 
@@ -128,14 +129,16 @@
     """Split arguments embedded to name or path like ``Example:arg1:arg2``.
 
     The separator can be either colon ``:`` or semicolon ``;``. If both are used,
     the first one is considered to be the separator.
     """
     if os.path.exists(name):
         return os.path.abspath(name), []
+    if isinstance(name, Path):
+        name = str(name)
     index = _get_arg_separator_index_from_name_or_path(name)
     if index == -1:
         return name, []
     args = name[index+1:].split(name[index])
     name = name[:index]
     if os.path.exists(name):
         name = os.path.abspath(name)
```

## Comparing `robotframework-6.1a1/src/robot/utils/unic.py` & `robotframework-6.1b1/src/robot/utils/unic.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/markuputils.py` & `robotframework-6.1b1/src/robot/utils/markuputils.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/robotpath.py` & `robotframework-6.1b1/src/robot/utils/robotpath.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/robottime.py` & `robotframework-6.1b1/src/robot/utils/robottime.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/encoding.py` & `robotframework-6.1b1/src/robot/utils/encoding.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 SYSTEM_ENCODING = get_system_encoding()
 PYTHONIOENCODING = os.getenv('PYTHONIOENCODING')
 
 
 def console_decode(string, encoding=CONSOLE_ENCODING):
     """Decodes bytes from console encoding to Unicode.
 
-    By default uses the system console encoding, but that can be configured
+    Uses the system console encoding by default, but that can be configured
     using the `encoding` argument. In addition to the normal encodings,
     it is possible to use case-insensitive values `CONSOLE` and `SYSTEM` to
     use the system console and system encoding, respectively.
 
     If `string` is already Unicode, it is returned as-is.
     """
     if is_string(string):
@@ -52,23 +52,25 @@
     """Encodes the given string so that it can be used in the console.
 
     If encoding is not given, determines it based on the given stream and system
     configuration. In addition to the normal encodings, it is possible to use
     case-insensitive values `CONSOLE` and `SYSTEM` to use the system console
     and system encoding, respectively.
 
-    By default decodes bytes back to Unicode because Python 3 APIs in general
+    Decodes bytes back to Unicode by default, because Python 3 APIs in general
     work with strings. Use `force=True` if that is not desired.
     """
+    if not is_string(string):
+        string = safe_str(string)
     if encoding:
         encoding = {'CONSOLE': CONSOLE_ENCODING,
                     'SYSTEM': SYSTEM_ENCODING}.get(encoding.upper(), encoding)
     else:
         encoding = _get_console_encoding(stream)
-    if encoding != 'UTF-8':
+    if encoding.upper() != 'UTF-8':
         encoded = string.encode(encoding, errors)
         return encoded if force else encoded.decode(encoding)
     return string.encode(encoding, errors) if force else string
 
 
 def _get_console_encoding(stream):
     encoding = getattr(stream, 'encoding', None)
```

## Comparing `robotframework-6.1a1/src/robot/utils/encodingsniffer.py` & `robotframework-6.1b1/src/robot/utils/encodingsniffer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/argumentparser.py` & `robotframework-6.1b1/src/robot/utils/argumentparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 import glob
 import os
 import re
 import shlex
 import sys
 import string
 import warnings
+from pathlib import Path
 
 from robot.errors import DataError, Information, FrameworkError
 from robot.version import get_full_version
 
 from .encoding import console_decode, system_decode
 from .filereader import FileReader
 from .misc import plural_or_not
 from .robottypes import is_falsy, is_integer, is_string
 
 
 def cmdline2list(args, escaping=False):
+    if isinstance(args, Path):
+        return [str(args)]
     lexer = shlex.shlex(args, posix=True)
     if is_falsy(escaping):
         lexer.escape = ''
     lexer.escapedquotes = '"\''
     lexer.commenters = ''
     lexer.whitespace_split = True
     try:
```

## Comparing `robotframework-6.1a1/src/robot/utils/asserts.py` & `robotframework-6.1b1/src/robot/utils/asserts.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/__init__.py` & `robotframework-6.1b1/src/robot/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from .connectioncache import ConnectionCache
 from .dotdict import DotDict
 from .encoding import (CONSOLE_ENCODING, SYSTEM_ENCODING, console_decode,
                        console_encode, system_decode, system_encode)
 from .error import (get_error_message, get_error_details, ErrorDetails)
 from .escaping import escape, glob_escape, unescape, split_from_equals
 from .etreewrapper import ET, ETSource
-from .filereader import FileReader
+from .filereader import FileReader, Source
 from .frange import frange
 from .markuputils import html_format, html_escape, xml_escape, attribute_escape
 from .markupwriters import HtmlWriter, XmlWriter, NullMarkupWriter
 from .importer import Importer
 from .match import eq, Matcher, MultiMatcher
 from .misc import (classproperty, isatty, parse_re_flags, plural_or_not,
                    printable_name, seq2str, seq2str2, test_or_task)
```

## Comparing `robotframework-6.1a1/src/robot/utils/application.py` & `robotframework-6.1b1/src/robot/utils/application.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/etreewrapper.py` & `robotframework-6.1b1/src/robot/utils/etreewrapper.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/match.py` & `robotframework-6.1b1/src/robot/utils/match.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,70 +12,73 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re
 import fnmatch
 from functools import partial
+from typing import Iterable, Iterator, Sequence
 
 from .normalizing import normalize
 from .robottypes import is_string
 
 
-def eq(str1, str2, ignore=(), caseless=True, spaceless=True):
+def eq(str1: str, str2: str, ignore: Sequence[str] = (), caseless: bool = True,
+       spaceless: bool = True) -> bool:
     str1 = normalize(str1, ignore, caseless, spaceless)
     str2 = normalize(str2, ignore, caseless, spaceless)
     return str1 == str2
 
 
 class Matcher:
 
-    def __init__(self, pattern, ignore=(), caseless=True, spaceless=True, regexp=False):
+    def __init__(self, pattern: str, ignore: Sequence[str] = (), caseless: bool = True,
+                 spaceless: bool = True, regexp: bool = False):
         self.pattern = pattern
         self._normalize = partial(normalize, ignore=ignore, caseless=caseless,
                                   spaceless=spaceless)
         self._regexp = self._compile(self._normalize(pattern), regexp=regexp)
 
     def _compile(self, pattern, regexp=False):
         if not regexp:
             pattern = fnmatch.translate(pattern)
         return re.compile(pattern, re.DOTALL)
 
-    def match(self, string):
+    def match(self, string: str) -> bool:
         return self._regexp.match(self._normalize(string)) is not None
 
-    def match_any(self, strings):
+    def match_any(self, strings: Sequence[str]) -> bool:
         return any(self.match(s) for s in strings)
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self._normalize(self.pattern))
 
 
-class MultiMatcher:
+class MultiMatcher(Iterable[Matcher]):
 
-    def __init__(self, patterns=None, ignore=(), caseless=True, spaceless=True,
-                 match_if_no_patterns=False, regexp=False):
-        self._matchers = [Matcher(pattern, ignore, caseless, spaceless, regexp)
-                          for pattern in self._ensure_list(patterns)]
-        self._match_if_no_patterns = match_if_no_patterns
+    def __init__(self, patterns: Iterable[str] = (), ignore: Sequence[str] = (),
+                 caseless: bool = True, spaceless: bool = True,
+                 match_if_no_patterns: bool = False, regexp: bool = False):
+        self.matchers = [Matcher(pattern, ignore, caseless, spaceless, regexp)
+                         for pattern in self._ensure_iterable(patterns)]
+        self.match_if_no_patterns = match_if_no_patterns
 
-    def _ensure_list(self, patterns):
+    def _ensure_iterable(self, patterns):
         if patterns is None:
-            return []
+            return ()
         if is_string(patterns):
-            return [patterns]
+            return (patterns,)
         return patterns
 
-    def match(self, string):
-        if self._matchers:
-            return any(m.match(string) for m in self._matchers)
-        return self._match_if_no_patterns
+    def match(self, string: str) -> bool:
+        if self.matchers:
+            return any(m.match(string) for m in self.matchers)
+        return self.match_if_no_patterns
 
-    def match_any(self, strings):
+    def match_any(self, strings: Sequence[str]) -> bool:
         return any(self.match(s) for s in strings)
 
-    def __len__(self):
-        return len(self._matchers)
+    def __len__(self) -> int:
+        return len(self.matchers)
 
-    def __iter__(self):
-        for matcher in self._matchers:
-            yield matcher.pattern
+    def __iter__(self) -> Iterator[Matcher]:
+        return iter(self.matchers)
```

## Comparing `robotframework-6.1a1/src/robot/utils/error.py` & `robotframework-6.1b1/src/robot/utils/error.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/robotenv.py` & `robotframework-6.1b1/src/robot/utils/robotenv.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/htmlformatters.py` & `robotframework-6.1b1/src/robot/utils/htmlformatters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/charwidth.py` & `robotframework-6.1b1/src/robot/utils/charwidth.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/platform.py` & `robotframework-6.1b1/src/robot/utils/platform.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/importer.py` & `robotframework-6.1b1/src/robot/utils/importer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/robotinspect.py` & `robotframework-6.1b1/src/robot/utils/robotinspect.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/utils/robottypes.py` & `robotframework-6.1b1/src/robot/utils/robottypes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/jsonwriter.py` & `robotframework-6.1b1/src/robot/htmldata/jsonwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/__init__.py` & `robotframework-6.1b1/src/robot/htmldata/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Package for writing output files in HTML format.
 
-This package is considered stable but it is not part of the public API.
+This package is considered stable, but it is not part of the public API.
 """
 
 from .htmlfilewriter import HtmlFileWriter, ModelWriter
 from .jsonwriter import JsonWriter
 
+
 LOG = 'rebot/log.html'
 REPORT = 'rebot/report.html'
 LIBDOC = 'libdoc/libdoc.html'
 TESTDOC = 'testdoc/testdoc.html'
```

## Comparing `robotframework-6.1a1/src/robot/htmldata/libdoc/libdoc.css` & `robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/libdoc/libdoc.html` & `robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.html`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/libdoc/pygments.css` & `robotframework-6.1b1/src/robot/htmldata/libdoc/pygments.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/libdoc/doc_formatting.css` & `robotframework-6.1b1/src/robot/htmldata/libdoc/doc_formatting.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/common.css` & `robotframework-6.1b1/src/robot/htmldata/rebot/common.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/report.css` & `robotframework-6.1b1/src/robot/htmldata/rebot/report.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/log.js` & `robotframework-6.1b1/src/robot/htmldata/rebot/log.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/print.css` & `robotframework-6.1b1/src/robot/htmldata/rebot/print.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/view.js` & `robotframework-6.1b1/src/robot/htmldata/rebot/view.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/report.html` & `robotframework-6.1b1/src/robot/htmldata/rebot/report.html`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/testdata.js` & `robotframework-6.1b1/src/robot/htmldata/rebot/testdata.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/util.js` & `robotframework-6.1b1/src/robot/htmldata/rebot/util.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/model.js` & `robotframework-6.1b1/src/robot/htmldata/rebot/model.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/log.html` & `robotframework-6.1b1/src/robot/htmldata/rebot/log.html`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/fileloading.js` & `robotframework-6.1b1/src/robot/htmldata/rebot/fileloading.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/doc_formatting.css` & `robotframework-6.1b1/src/robot/htmldata/rebot/doc_formatting.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/rebot/log.css` & `robotframework-6.1b1/src/robot/htmldata/rebot/log.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/lib/jsxcompressor.min.js` & `robotframework-6.1b1/src/robot/htmldata/lib/jsxcompressor.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/lib/jquery.tablesorter.min.js` & `robotframework-6.1b1/src/robot/htmldata/lib/jquery.tablesorter.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/lib/jquery.highlight.min.js` & `robotframework-6.1b1/src/robot/htmldata/lib/jquery.highlight.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/lib/jquery.min.js` & `robotframework-6.1b1/src/robot/htmldata/lib/jquery.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/lib/jquery.tmpl.min.js` & `robotframework-6.1b1/src/robot/htmldata/lib/jquery.tmpl.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/testdoc/testdoc.html` & `robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.html`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/htmldata/common/storage.js` & `robotframework-6.1b1/src/robot/htmldata/common/storage.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/parsing/suitestructure.py` & `robotframework-6.1b1/src/robot/parsing/suitestructure.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,158 +9,176 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from os.path import normpath
+from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List
+from typing import Iterable, Sequence
 
 from robot.errors import DataError
 from robot.model import SuiteNamePatterns
 from robot.output import LOGGER
-from robot.utils import get_error_message, seq2str
+from robot.utils import get_error_message
 
 
-class SuiteStructure:
+class SuiteStructure(ABC):
+    source: 'Path|None'
+    init_file: 'Path|None'
+    children: 'list[SuiteStructure]|None'
 
-    def __init__(self, source: Path = None, init_file: Path = None,
-                 children: List['SuiteStructure'] = None):
+    def __init__(self, source: 'Path|None', init_file: 'Path|None' = None,
+                 children: 'Sequence[SuiteStructure]|None' = None):
         self.source = source
         self.init_file = init_file
-        self.children = children
+        self.children = list(children) if children is not None else None
 
     @property
-    def extension(self):
-        source = self.source if self.is_file else self.init_file
-        return source.suffix[1:].lower() if source else None
+    @abstractmethod
+    def extension(self) -> 'str|None':
+        raise NotImplementedError
+
+    @abstractmethod
+    def visit(self, visitor: 'SuiteStructureVisitor'):
+        raise NotImplementedError
+
+
+class SuiteFile(SuiteStructure):
+    source: Path
+
+    def __init__(self, source: Path):
+        super().__init__(source)
+
+    @property
+    def extension(self) -> str:
+        return self.source.suffix[1:].lower()
+
+    def visit(self, visitor: 'SuiteStructureVisitor'):
+        visitor.visit_file(self)
+
+
+class SuiteDirectory(SuiteStructure):
+    children: 'list[SuiteStructure]'
+
+    def __init__(self, source: 'Path|None' = None, init_file: 'Path|None' = None,
+                 children: Sequence[SuiteStructure] = ()):
+        super().__init__(source, init_file, children)
 
     @property
-    def is_file(self):
-        return self.children is None
+    def is_multi_source(self) -> bool:
+        return self.source is None
+
+    @property
+    def extension(self) -> 'str|None':
+        return self.init_file.suffix[1:].lower() if self.init_file else None
 
     def add(self, child: 'SuiteStructure'):
         self.children.append(child)
 
-    def visit(self, visitor):
-        if self.children is None:
-            visitor.visit_file(self)
-        else:
-            visitor.visit_directory(self)
+    def visit(self, visitor: 'SuiteStructureVisitor'):
+        visitor.visit_directory(self)
 
 
 class SuiteStructureVisitor:
 
-    def visit_file(self, structure):
+    def visit_file(self, structure: SuiteFile):
         pass
 
-    def visit_directory(self, structure):
+    def visit_directory(self, structure: SuiteDirectory):
         self.start_directory(structure)
         for child in structure.children:
             child.visit(self)
         self.end_directory(structure)
 
-    def start_directory(self, structure):
+    def start_directory(self, structure: SuiteDirectory):
         pass
 
-    def end_directory(self, structure):
+    def end_directory(self, structure: SuiteDirectory):
         pass
 
 
 class SuiteStructureBuilder:
     ignored_prefixes = ('_', '.')
     ignored_dirs = ('CVS',)
 
-    def __init__(self, included_extensions=('.robot', '.rbt'), included_suites=None):
-        self.included_extensions = included_extensions
-        self.included_suites = None if not included_suites else \
-            SuiteNamePatterns(self._create_included_suites(included_suites))
+    def __init__(self, extensions: Iterable[str] = ('.robot', '.rbt'),
+                 included_suites: Iterable[str] = ()):
+        self.extensions = {'.' + ext.lstrip('.').lower() for ext in extensions}
+        self.included_suites = SuiteNamePatterns(
+            self._create_included_suites(included_suites)
+        )
 
     def _create_included_suites(self, included_suites):
         for suite in included_suites:
             yield suite
             while '.' in suite:
                 suite = suite.split('.', 1)[1]
                 yield suite
 
-    def build(self, paths):
-        paths = list(self._normalize_paths(paths))
+    def build(self, *paths: Path) -> SuiteStructure:
         if len(paths) == 1:
             return self._build(paths[0], self.included_suites)
         return self._build_multi_source(paths)
 
-    def _normalize_paths(self, paths):
-        if not paths:
-            raise DataError('One or more source paths required.')
-        # Cannot use `Path.resolve()` here because it resolves all symlinks which
-        # isn't desired. `Path` doesn't have any methods for normalizing paths
-        # so need to use `os.path.normpath()`. Also that _may_ resolve symlinks,
-        # but we need to do it for backwards compatibility.
-        paths = [Path(normpath(p)).absolute() for p in paths]
-        non_existing = [p for p in paths if not p.exists()]
-        if non_existing:
-            raise DataError(f"Parsing {seq2str(non_existing)} failed: "
-                            f"File or directory to execute does not exist.")
-        return paths
-
-    def _build(self, path, included_suites):
+    def _build(self, path: Path, included_suites: SuiteNamePatterns) -> SuiteStructure:
         if path.is_file():
-            return SuiteStructure(path)
+            return SuiteFile(path)
         return self._build_directory(path, included_suites)
 
-    def _build_directory(self, dir_path, included_suites):
-        structure = SuiteStructure(dir_path, children=[])
+    def _build_directory(self, path: Path,
+                         included_suites: SuiteNamePatterns) -> SuiteStructure:
+        structure = SuiteDirectory(path)
         # If a directory is included, also its children are included.
-        if self._is_suite_included(dir_path.name, included_suites):
-            included_suites = None
-        for path in self._list_dir(dir_path):
-            if self._is_init_file(path):
+        if self._is_suite_included(path.name, included_suites):
+            included_suites = SuiteNamePatterns()
+        for item in self._list_dir(path):
+            if self._is_init_file(item):
                 if structure.init_file:
-                    LOGGER.error(f"Ignoring second test suite init file '{path}'.")
+                    LOGGER.error(f"Ignoring second test suite init file '{item}'.")
                 else:
-                    structure.init_file = path
-            elif self._is_included(path, included_suites):
-                structure.add(self._build(path, included_suites))
+                    structure.init_file = item
+            elif self._is_included(item, included_suites):
+                structure.add(self._build(item, included_suites))
             else:
-                LOGGER.info(f"Ignoring file or directory '{path}'.")
+                LOGGER.info(f"Ignoring file or directory '{item}'.")
         return structure
 
-    def _is_suite_included(self, name, included_suites):
+    def _is_suite_included(self, name: str, included_suites: SuiteNamePatterns) -> bool:
         if not included_suites:
             return True
         if '__' in name:
             name = name.split('__', 1)[1] or name
         return included_suites.match(name)
 
-    def _list_dir(self, path):
+    def _list_dir(self, path: Path) -> 'list[Path]':
         try:
             return sorted(path.iterdir(), key=lambda p: p.name.lower())
         except OSError:
             raise DataError(f"Reading directory '{path}' failed: {get_error_message()}")
 
-    def _is_init_file(self, path: Path):
+    def _is_init_file(self, path: Path) -> bool:
         return (path.stem.lower() == '__init__'
-                and path.suffix.lower() in self.included_extensions
+                and path.suffix.lower() in self.extensions
                 and path.is_file())
 
-    def _is_included(self, path: Path, included_suites):
+    def _is_included(self, path: Path, included_suites: SuiteNamePatterns) -> bool:
         if path.name.startswith(self.ignored_prefixes):
             return False
         if path.is_dir():
             return path.name not in self.ignored_dirs
         if not path.is_file():
             return False
-        if path.suffix.lower() not in self.included_extensions:
+        if path.suffix.lower() not in self.extensions:
             return False
         return self._is_suite_included(path.stem, included_suites)
 
-    def _build_multi_source(self, paths: List[Path]):
-        structure = SuiteStructure(children=[])
+    def _build_multi_source(self, paths: Iterable[Path]) -> SuiteStructure:
+        structure = SuiteDirectory()
         for path in paths:
             if self._is_init_file(path):
                 if structure.init_file:
                     raise DataError("Multiple init files not allowed.")
                 structure.init_file = path
             else:
                 structure.add(self._build(path, self.included_suites))
```

## Comparing `robotframework-6.1a1/src/robot/parsing/__init__.py` & `robotframework-6.1b1/src/robot/parsing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 this module directly, issue should be submitted about exposing it explicitly via
 :mod:`robot.api.parsing`.
 """
 
 from .lexer import get_tokens, get_resource_tokens, get_init_tokens, Token
 from .model import File, ModelTransformer, ModelVisitor
 from .parser import get_model, get_resource_model, get_init_model
-from .suitestructure import SuiteStructureBuilder, SuiteStructureVisitor
+from .suitestructure import (SuiteFile, SuiteDirectory, SuiteStructure,
+                             SuiteStructureBuilder, SuiteStructureVisitor)
```

## Comparing `robotframework-6.1a1/src/robot/parsing/model/blocks.py` & `robotframework-6.1b1/src/robot/parsing/model/blocks.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,174 +9,203 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import ast
+from abc import ABC
 from contextlib import contextmanager
-
-from robot.utils import file_writer, is_pathlike, is_string
-
-from .statements import (Break, Continue, Error, KeywordCall, ReturnSetting,
-                         ReturnStatement, Statement, TemplateArguments)
+from io import IOBase
+from pathlib import Path
+from typing import cast, Iterator, Sequence, Union
+
+from robot.utils import file_writer, test_or_task
+
+from .statements import (Break, Continue, ElseHeader, ElseIfHeader, End, ExceptHeader,
+                         Error, FinallyHeader, ForHeader, IfHeader, KeywordCall,
+                         KeywordName, Node, ReturnSetting, ReturnStatement,
+                         SectionHeader, Statement, TemplateArguments, TestCaseName,
+                         TryHeader, WhileHeader)
 from .visitor import ModelVisitor
 from ..lexer import Token
 
 
-class Block(ast.AST):
-    _fields = ()
-    _attributes = ('lineno', 'col_offset', 'end_lineno', 'end_col_offset', 'errors')
-    errors = ()
+Body = Sequence[Union[Statement, 'Block']]
+Errors = Sequence[str]
+
+
+class Container(Node, ABC):
 
     @property
-    def lineno(self):
+    def lineno(self) -> int:
         statement = FirstStatementFinder.find_from(self)
         return statement.lineno if statement else -1
 
     @property
-    def col_offset(self):
+    def col_offset(self) -> int:
         statement = FirstStatementFinder.find_from(self)
         return statement.col_offset if statement else -1
 
     @property
-    def end_lineno(self):
+    def end_lineno(self) -> int:
         statement = LastStatementFinder.find_from(self)
         return statement.end_lineno if statement else -1
 
     @property
-    def end_col_offset(self):
+    def end_col_offset(self) -> int:
         statement = LastStatementFinder.find_from(self)
         return statement.end_col_offset if statement else -1
 
     def validate_model(self):
         ModelValidator().visit(self)
 
     def validate(self, ctx: 'ValidationContext'):
         pass
 
 
-class HeaderAndBody(Block):
-    _fields = ('header', 'body')
-
-    def __init__(self, header=None, body=None, errors=()):
-        self.header = header
-        self.body = body or []
-        self.errors = errors
-
-    def _body_is_empty(self):
-        # This works with tests, keywords and blocks inside them, not with sections.
-        valid = (KeywordCall, TemplateArguments, Continue, ReturnStatement, Break,
-                 Block, Error)
-        return not any(isinstance(node, valid) for node in self.body)
-
-
-class File(Block):
+class File(Container):
     _fields = ('sections',)
-    _attributes = ('source', 'languages') + Block._attributes
+    _attributes = ('source', 'languages') + Container._attributes
 
-    def __init__(self, sections=None, source=None, languages=()):
-        self.sections = sections or []
+    def __init__(self, sections: 'Sequence[Section]' = (), source: 'Path|None' = None,
+                 languages: Sequence[str] = ()):
+        super().__init__()
+        self.sections = list(sections)
         self.source = source
-        self.languages = languages
+        self.languages = list(languages)
 
-    def save(self, output=None):
+    def save(self, output: 'Path|str|IOBase|None' = None):
         """Save model to the given ``output`` or to the original source file.
 
         The ``output`` can be a path to a file or an already opened file
         object. If ``output`` is not given, the original source file will
         be overwritten.
         """
         output = output or self.source
         if output is None:
             raise TypeError('Saving model requires explicit output '
                             'when original source is not path.')
         ModelWriter(output).write(self)
 
 
-class Section(HeaderAndBody):
-    pass
+class Block(Container, ABC):
+    _fields = ('header', 'body')
+
+    def __init__(self, header: 'Statement|None', body: Body = (), errors: Errors = ()):
+        self.header = header
+        self.body = list(body)
+        self.errors = tuple(errors)
+
+    def _body_is_empty(self):
+        # This works with tests, keywords, and blocks inside them, not with sections.
+        valid = (KeywordCall, TemplateArguments, Continue, Break, ReturnSetting,
+                 ReturnStatement, NestedBlock, Error)
+        return not any(isinstance(node, valid) for node in self.body)
+
+
+class Section(Block):
+    header: 'SectionHeader|None'
 
 
 class SettingSection(Section):
-    pass
+    header: SectionHeader
 
 
 class VariableSection(Section):
-    pass
+    header: SectionHeader
 
 
 # TODO: should there be a separate TaskSection?
 class TestCaseSection(Section):
+    header: SectionHeader
 
     @property
-    def tasks(self):
+    def tasks(self) -> bool:
         return self.header.type == Token.TASK_HEADER
 
 
 class KeywordSection(Section):
-    pass
+    header: SectionHeader
 
 
 class CommentSection(Section):
-    pass
+    header: 'SectionHeader|None'
+
+
+class ImplicitCommentSection(CommentSection):
+    header: None
+
+    def __init__(self, header: 'Statement|None' = None, body: Body = (),
+                 errors: Errors = ()):
+        body = ([header] if header is not None else []) + list(body)
+        super().__init__(None, body, errors)
 
 
 class InvalidSection(Section):
     pass
 
 
-class TestCase(HeaderAndBody):
+class TestCase(Block):
+    header: TestCaseName
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.header.name
 
     def validate(self, ctx: 'ValidationContext'):
         if self._body_is_empty():
-            # FIXME: Tasks!
-            self.errors += ('Test contains no keywords.',)
+            self.errors += (test_or_task('{Test} cannot be empty.', ctx.tasks),)
 
 
-class Keyword(HeaderAndBody):
+class Keyword(Block):
+    header: KeywordName
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.header.name
 
     def validate(self, ctx: 'ValidationContext'):
         if self._body_is_empty():
-            if not any(isinstance(node, ReturnSetting) for node in self.body):
-                self.errors += (f"User keyword '{self.name}' contains no keywords.",)
+            self.errors += ("User keyword cannot be empty.",)
 
 
-class If(HeaderAndBody):
+class NestedBlock(Block):
+    _fields = ('header', 'body', 'end')
+
+    def __init__(self, header: Statement, body: Body = (), end: 'End|None' = None,
+                 errors: Errors = ()):
+        super().__init__(header, body, errors)
+        self.end = end
+
+
+class If(NestedBlock):
     """Represents IF structures in the model.
 
     Used with IF, Inline IF, ELSE IF and ELSE nodes. The :attr:`type` attribute
     specifies the type.
     """
     _fields = ('header', 'body', 'orelse', 'end')
+    header: 'IfHeader|ElseIfHeader|ElseHeader'
 
-    def __init__(self, header, body=None, orelse=None, end=None, errors=()):
-        super().__init__(header, body, errors)
+    def __init__(self, header: Statement, body: Body = (), orelse: 'If|None' = None,
+                 end: 'End|None' = None, errors: Errors = ()):
+        super().__init__(header, body, end, errors)
         self.orelse = orelse
-        self.end = end
 
     @property
-    def type(self):
+    def type(self) -> str:
         return self.header.type
 
     @property
-    def condition(self):
+    def condition(self) -> 'str|None':
         return self.header.condition
 
     @property
-    def assign(self):
+    def assign(self) -> 'tuple[str, ...]':
         return self.header.assign
 
     def validate(self, ctx: 'ValidationContext'):
         self._validate_body()
         if self.type == Token.IF:
             self._validate_structure()
             self._validate_end()
@@ -208,85 +237,82 @@
             self.errors += ('IF must have closing END.',)
 
     def _validate_inline_if(self):
         branch = self
         assign = branch.assign
         while branch:
             if branch.body:
-                item = branch.body[0]
+                item = cast(Statement, branch.body[0])
                 if assign and item.type != Token.KEYWORD:
                     self.errors += ('Inline IF with assignment can only contain '
                                     'keyword calls.',)
                 if getattr(item, 'assign', None):
                     self.errors += ('Inline IF branches cannot contain assignments.',)
                 if item.type == Token.INLINE_IF:
                     self.errors += ('Inline IF cannot be nested.',)
             branch = branch.orelse
 
 
-class For(HeaderAndBody):
-    _fields = ('header', 'body', 'end')
-
-    def __init__(self, header, body=None, end=None, errors=()):
-        super().__init__(header, body, errors)
-        self.end = end
+class For(NestedBlock):
+    header: ForHeader
 
     @property
-    def variables(self):
+    def variables(self) -> 'tuple[str, ...]':
         return self.header.variables
 
     @property
-    def values(self):
+    def values(self) -> 'tuple[str, ...]':
         return self.header.values
 
     @property
-    def flavor(self):
+    def flavor(self) -> 'str|None':
         return self.header.flavor
 
     @property
-    def start(self):
+    def start(self) -> 'str|None':
         return self.header.start
 
     @property
-    def mode(self):
+    def mode(self) -> 'str|None':
         return self.header.mode
 
     @property
-    def fill(self):
+    def fill(self) -> 'str|None':
         return self.header.fill
 
     def validate(self, ctx: 'ValidationContext'):
         if self._body_is_empty():
             self.errors += ('FOR loop cannot be empty.',)
         if not self.end:
             self.errors += ('FOR loop must have closing END.',)
 
 
-class Try(HeaderAndBody):
+class Try(NestedBlock):
     _fields = ('header', 'body', 'next', 'end')
+    header: 'TryHeader|ExceptHeader|ElseHeader|FinallyHeader'
 
-    def __init__(self, header, body=None, next=None, end=None, errors=()):
-        super().__init__(header, body, errors)
+    def __init__(self, header: Statement, body: Body = (), next: 'Try|None' = None,
+                 end: 'End|None' = None, errors: Errors = ()):
+        super().__init__(header, body, end, errors)
         self.next = next
-        self.end = end
 
     @property
-    def type(self):
+    def type(self) -> str:
         return self.header.type
 
     @property
-    def patterns(self):
+    def patterns(self) -> 'tuple[str, ...]':
         return getattr(self.header, 'patterns', ())
 
     @property
-    def pattern_type(self):
+    def pattern_type(self) -> 'str|None':
         return getattr(self.header, 'pattern_type', None)
 
     @property
-    def variable(self):
+    def variable(self) -> 'str|None':
         return getattr(self.header, 'variable', None)
 
     def validate(self, ctx: 'ValidationContext'):
         self._validate_body()
         if self.type == Token.TRY:
             self._validate_structure()
             self._validate_end()
@@ -329,55 +355,59 @@
             self.errors += ('TRY structure must have EXCEPT or FINALLY branch.',)
 
     def _validate_end(self):
         if not self.end:
             self.errors += ('TRY must have closing END.',)
 
 
-class While(HeaderAndBody):
-    _fields = ('header', 'body', 'end')
-
-    def __init__(self, header, body=None, end=None, errors=()):
-        super().__init__(header, body, errors)
-        self.end = end
+class While(NestedBlock):
+    header: WhileHeader
 
     @property
-    def condition(self):
+    def condition(self) -> str:
         return self.header.condition
 
     @property
-    def limit(self):
+    def limit(self) -> 'str|None':
         return self.header.limit
 
+    @property
+    def on_limit(self) -> 'str|None':
+        return self.header.on_limit
+
+    @property
+    def on_limit_message(self) -> 'str|None':
+        return self.header.on_limit_message
+
     def validate(self, ctx: 'ValidationContext'):
         if self._body_is_empty():
             self.errors += ('WHILE loop cannot be empty.',)
         if not self.end:
             self.errors += ('WHILE loop must have closing END.',)
 
 
 class ModelWriter(ModelVisitor):
 
-    def __init__(self, output):
-        if is_string(output) or is_pathlike(output):
+    def __init__(self, output: 'Path|str|IOBase'):
+        if isinstance(output, (Path, str)):
             self.writer = file_writer(output)
             self.close_writer = True
         else:
             self.writer = output
             self.close_writer = False
 
-    def write(self, model: Block):
+    def write(self, model: Node):
         try:
             self.visit(model)
         finally:
             if self.close_writer:
                 self.writer.close()
 
     def visit_Statement(self, statement: Statement):
-        for token in statement.tokens:
+        for token in statement:
             self.writer.write(token.value)
 
 
 class ModelValidator(ModelVisitor):
 
     def __init__(self):
         self.ctx = ValidationContext()
@@ -393,65 +423,72 @@
 
 class ValidationContext:
 
     def __init__(self):
         self.blocks = []
 
     @contextmanager
-    def block(self, node: Block):
+    def block(self, node: Block) -> Iterator[None]:
         self.blocks.append(node)
         try:
             yield
         finally:
             self.blocks.pop()
 
     @property
-    def parent_block(self):
+    def parent_block(self) -> 'Block|None':
         return self.blocks[-1] if self.blocks else None
 
     @property
-    def in_keyword(self):
+    def tasks(self) -> bool:
+        for parent in self.blocks:
+            if isinstance(parent, TestCaseSection):
+                return parent.tasks
+        return False
+
+    @property
+    def in_keyword(self) -> bool:
         return any(isinstance(b, Keyword) for b in self.blocks)
 
     @property
-    def in_loop(self):
+    def in_loop(self) -> bool:
         return any(isinstance(b, (For, While)) for b in self.blocks)
 
     @property
-    def in_finally(self):
+    def in_finally(self) -> bool:
         parent = self.parent_block
         return isinstance(parent, Try) and parent.header.type == Token.FINALLY
 
 
 class FirstStatementFinder(ModelVisitor):
 
     def __init__(self):
-        self.statement = None
+        self.statement: 'Statement|None' = None
 
     @classmethod
-    def find_from(cls, model):
+    def find_from(cls, model: Node) -> 'Statement|None':
         finder = cls()
         finder.visit(model)
         return finder.statement
 
-    def visit_Statement(self, statement):
+    def visit_Statement(self, statement: Statement):
         if self.statement is None:
             self.statement = statement
 
-    def generic_visit(self, node):
+    def generic_visit(self, node: Node):
         if self.statement is None:
-            ModelVisitor.generic_visit(self, node)
+            super().generic_visit(node)
 
 
 class LastStatementFinder(ModelVisitor):
 
     def __init__(self):
-        self.statement = None
+        self.statement: 'Statement|None' = None
 
     @classmethod
-    def find_from(cls, model):
+    def find_from(cls, model: Node) -> 'Statement|None':
         finder = cls()
         finder.visit(model)
         return finder.statement
 
-    def visit_Statement(self, statement):
+    def visit_Statement(self, statement: Statement):
         self.statement = statement
```

## Comparing `robotframework-6.1a1/src/robot/parsing/model/__init__.py` & `robotframework-6.1b1/src/robot/parsing/model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .blocks import (File, SettingSection, VariableSection, TestCaseSection,
-                     KeywordSection, CommentSection, InvalidSection,
-                     TestCase, Keyword, For, If, Try, While)
-from .statements import Statement
+from .blocks import (Block, CommentSection, Container, File, For, If,
+                     ImplicitCommentSection, InvalidSection, Keyword,
+                     KeywordSection, NestedBlock, Section, SettingSection,
+                     TestCase, TestCaseSection, Try, VariableSection, While)
+from .statements import Config, End, Statement
 from .visitor import ModelTransformer, ModelVisitor
```

## Comparing `robotframework-6.1a1/src/robot/parsing/model/visitor.py` & `robotframework-6.1b1/src/robot/parsing/model/visitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import ast
 
+from .statements import Node
+
 
 class VisitorFinder:
 
     def _find_visitor(self, cls):
         if cls is ast.AST:
             return None
         method = 'visit_' + cls.__name__
         if hasattr(self, method):
             return getattr(self, method)
         # Forward-compatibility.
         if method == 'visit_Return' and hasattr(self, 'visit_ReturnSetting'):
-            return self.visit_ReturnSetting
+            return getattr(self, 'visit_ReturnSetting')
         for base in cls.__bases__:
             visitor = self._find_visitor(base)
             if visitor:
                 return visitor
         return None
 
 
@@ -43,23 +45,23 @@
     is one of the base classes of the node. For example, this visitor method
     matches all ``Statement`` nodes::
 
         def visit_Statement(self, node):
             ...
     """
 
-    def visit(self, node):
+    def visit(self, node: Node):
         visitor = self._find_visitor(type(node)) or self.generic_visit
         visitor(node)
 
 
 class ModelTransformer(ast.NodeTransformer, VisitorFinder):
     """NodeTransformer that supports matching nodes based on their base classes.
 
     See :class:`ModelVisitor` for explanation how this is different compared
     to the standard `ast.NodeTransformer
     <https://docs.python.org/library/ast.html#ast.NodeTransformer>`__.
     """
 
-    def visit(self, node):
+    def visit(self, node: Node):
         visitor = self._find_visitor(type(node)) or self.generic_visit
         return visitor(node)
```

## Comparing `robotframework-6.1a1/src/robot/parsing/model/statements.py` & `robotframework-6.1b1/src/robot/parsing/model/statements.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,255 +11,335 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import ast
 import re
-from typing import TYPE_CHECKING
+from abc import ABC, abstractmethod
+from collections.abc import Iterator, Sequence
+from typing import cast, ClassVar, overload, TYPE_CHECKING, Type, TypeVar
 
 from robot.conf import Language
 from robot.running.arguments import UserKeywordArgumentParser
-from robot.utils import is_list_like, normalize_whitespace, seq2str, split_from_equals
+from robot.utils import normalize_whitespace, seq2str, split_from_equals, test_or_task
 from robot.variables import is_scalar_assign, is_dict_variable, search_variable
 
 from ..lexer import Token
 
 if TYPE_CHECKING:
     from .blocks import ValidationContext
 
 
+T = TypeVar('T', bound='Statement')
 FOUR_SPACES = '    '
 EOL = '\n'
 
 
-class Statement(ast.AST):
-    type = None
-    handles_types = ()
-    _fields = ('type', 'tokens')
+class Node(ast.AST, ABC):
     _attributes = ('lineno', 'col_offset', 'end_lineno', 'end_col_offset', 'errors')
-    _statement_handlers = {}
+    lineno: int
+    col_offset: int
+    end_lineno: int
+    end_col_offset: int
+    errors: 'tuple[str, ...]' = ()
+
+
+class Statement(Node, ABC):
+    _fields = ('type', 'tokens')
+    type: str
+    handles_types: 'ClassVar[tuple[str, ...]]' = ()
+    statement_handlers: 'ClassVar[dict[str, Type[Statement]]]' = {}
 
-    def __init__(self, tokens, errors=()):
+    def __init__(self, tokens: 'Sequence[Token]', errors: 'Sequence[str]' = ()):
         self.tokens = tuple(tokens)
-        self.errors = errors
+        self.errors = tuple(errors)
 
     @property
-    def lineno(self):
+    def lineno(self) -> int:
         return self.tokens[0].lineno if self.tokens else -1
 
     @property
-    def col_offset(self):
+    def col_offset(self) -> int:
         return self.tokens[0].col_offset if self.tokens else -1
 
     @property
-    def end_lineno(self):
+    def end_lineno(self) -> int:
         return self.tokens[-1].lineno if self.tokens else -1
 
     @property
-    def end_col_offset(self):
+    def end_col_offset(self) -> int:
         return self.tokens[-1].end_col_offset if self.tokens else -1
 
     @classmethod
-    def register(cls, subcls):
+    def register(cls, subcls: Type[T]) -> Type[T]:
         types = subcls.handles_types or (subcls.type,)
         for typ in types:
-            cls._statement_handlers[typ] = subcls
+            cls.statement_handlers[typ] = subcls
         return subcls
 
     @classmethod
-    def from_tokens(cls, tokens):
-        handlers = cls._statement_handlers
+    def from_tokens(cls, tokens: 'Sequence[Token]') -> 'Statement':
+        """Create a statement from given tokens.
+
+        Statement type is got automatically from token types.
+
+        This classmethod should be called from :class:`Statement`, not from
+        its subclasses. If you know the subclass to use, simply create an
+        instance of it directly.
+        """
+        handlers = cls.statement_handlers
         for token in tokens:
             if token.type in handlers:
                 return handlers[token.type](tokens)
         if any(token.type == Token.ASSIGN for token in tokens):
             return KeywordCall(tokens)
         return EmptyLine(tokens)
 
     @classmethod
-    def from_params(cls, *args, **kwargs):
-        """Create statement from passed parameters.
-
-        Required and optional arguments should match class properties. Values are
-        used to create matching tokens.
+    @abstractmethod
+    def from_params(cls, *args, **kwargs) -> 'Statement':
+        """Create a statement from passed parameters.
 
-        There is one notable difference for `Documentation` statement where
-        ``settings_header`` flag is used to determine if statement belongs to
-        settings header or test/keyword.
+        Required and optional arguments in general match class properties.
+        Values are used to create matching tokens.
 
         Most implementations support following general properties:
 
         - ``separator`` whitespace inserted between each token. Default is four spaces.
         - ``indent`` whitespace inserted before first token. Default is four spaces.
         - ``eol`` end of line sign. Default is ``'\\n'``.
+
+        This classmethod should be called from the :class:`Statement` subclass
+        to create, not from the :class:`Statement` class itself.
         """
         raise NotImplementedError
 
     @property
-    def data_tokens(self):
+    def data_tokens(self) -> 'list[Token]':
         return [t for t in self.tokens if t.type not in Token.NON_DATA_TOKENS]
 
-    def get_token(self, *types):
-        """Return a token with the given ``type``.
+    def get_token(self, *types: str) -> 'Token|None':
+        """Return a token with any of the given ``types``.
 
         If there are no matches, return ``None``. If there are multiple
         matches, return the first match.
         """
         for token in self.tokens:
             if token.type in types:
                 return token
         return None
 
-    def get_tokens(self, *types):
+    def get_tokens(self, *types: str) -> 'list[Token]':
         """Return tokens having any of the given ``types``."""
         return [t for t in self.tokens if t.type in types]
 
-    def get_value(self, type, default=None):
+    @overload
+    def get_value(self, type: str, default: str) -> str:
+        ...
+
+    @overload
+    def get_value(self, type: str, default: None = None) -> 'str|None':
+        ...
+
+    def get_value(self, type: str, default: 'str|None' = None) -> 'str|None':
         """Return value of a token with the given ``type``.
 
         If there are no matches, return ``default``. If there are multiple
         matches, return the value of the first match.
         """
         token = self.get_token(type)
         return token.value if token else default
 
-    def get_values(self, *types):
+    def get_values(self, *types: str) -> 'tuple[str, ...]':
         """Return values of tokens having any of the given ``types``."""
         return tuple(t.value for t in self.tokens if t.type in types)
 
-    def get_option(self, name):
-        options = dict(opt.split('=', 1) for opt in self.get_values(Token.OPTION))
-        return options.get(name)
+    def get_option(self, name: str, default: 'str|None' = None) -> 'str|None':
+        """Return value of a configuration option with the given ``name``.
+
+        If the option has not been used, return ``default``.
+
+        If the option has been used multiple times, values are joined together.
+        This is typically an error situation and validated elsewhere.
+
+        New in Robot Framework 6.1.
+        """
+        options = self._get_options()
+        return ', '.join(options[name]) if name in options else default
+
+    def _get_options(self) -> 'dict[str, list[str]]':
+        options: 'dict[str, list[str]]' = {}
+        for option in self.get_values(Token.OPTION):
+            name, value = option.split('=', 1)
+            options.setdefault(name, []).append(value)
+        return options
 
     @property
-    def lines(self):
+    def lines(self) -> 'Iterator[list[Token]]':
         line = []
         for token in self.tokens:
             line.append(token)
             if token.type == Token.EOL:
                 yield line
                 line = []
         if line:
             yield line
 
     def validate(self, ctx: 'ValidationContext'):
         pass
 
-    def __iter__(self):
+    def _validate_options(self):
+        for name, values in self._get_options().items():
+            if len(values) > 1:
+                self.errors += (f"Option '{name}' allowed only once, got values "
+                                f"{seq2str(values)}.",)
+
+    def __iter__(self) -> 'Iterator[Token]':
         return iter(self.tokens)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.tokens)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> Token:
         return self.tokens[item]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         name = type(self).__name__
         tokens = f'tokens={list(self.tokens)}'
         errors = f', errors={list(self.errors)}' if self.errors else ''
         return f'{name}({tokens}{errors})'
 
 
-class DocumentationOrMetadata(Statement):
+class DocumentationOrMetadata(Statement, ABC):
+
+    @property
+    def value(self) -> str:
+        return ''.join(self._get_lines()).rstrip()
+
+    def _get_lines(self) -> 'Iterator[str]':
+        base_offset = -1
+        for tokens in self._get_line_tokens():
+            yield from self._get_line_values(tokens, base_offset)
+            first = tokens[0]
+            if base_offset < 0 or 0 < first.col_offset < base_offset and first.value:
+                base_offset = first.col_offset
 
-    def _join_value(self, tokens):
-        lines = self._get_lines(tokens)
-        return ''.join(self._yield_lines_with_newlines(lines))
-
-    def _get_lines(self, tokens):
-        lines = []
-        line = None
+    def _get_line_tokens(self) -> 'Iterator[list[Token]]':
+        line: 'list[Token]' = []
         lineno = -1
-        for t in tokens:
-            if t.lineno != lineno:
+        # There are no EOLs during execution or if data has been parsed with
+        # `data_only=True` otherwise, so we need to look at line numbers to
+        # know when lines change. If model is created programmatically using
+        # `from_params` or otherwise, line numbers may not be set, but there
+        # ought to be EOLs. If both EOLs and line numbers are missing,
+        # everything is considered to be on the same line.
+        for token in self.get_tokens(Token.ARGUMENT, Token.EOL):
+            eol = token.type == Token.EOL
+            if token.lineno != lineno or eol:
+                if line:
+                    yield line
                 line = []
-                lines.append(line)
-            line.append(t.value)
-            lineno = t.lineno
-        return [' '.join(line) for line in lines]
-
-    def _yield_lines_with_newlines(self, lines):
-        last_index = len(lines) - 1
-        for index, line in enumerate(lines):
+            if not eol:
+                line.append(token)
+            lineno = token.lineno
+        if line:
             yield line
-            if index < last_index and not self._escaped_or_has_newline(line):
-                yield '\n'
 
-    def _escaped_or_has_newline(self, line):
+    def _get_line_values(self, tokens: 'list[Token]', offset: int) -> 'Iterator[str]':
+        token = None
+        for index, token in enumerate(tokens):
+            if token.col_offset > offset > 0:
+                yield ' ' * (token.col_offset - offset)
+            elif index > 0:
+                yield ' '
+            yield self._remove_trailing_backslash(token.value)
+            offset = token.end_col_offset
+        if token and not self._has_trailing_backslash_or_newline(token.value):
+            yield '\n'
+
+    def _remove_trailing_backslash(self, value: str) -> str:
+        if value and value[-1] == '\\':
+            match = re.search(r'(\\+)$', value)
+            if match and len(match.group(1)) % 2 == 1:
+                value = value[:-1]
+        return value
+
+    def _has_trailing_backslash_or_newline(self, line: str) -> bool:
         match = re.search(r'(\\+)n?$', line)
-        return match and len(match.group(1)) % 2 == 1
+        return bool(match and len(match.group(1)) % 2 == 1)
 
 
-class SingleValue(Statement):
+class SingleValue(Statement, ABC):
 
     @property
-    def value(self):
+    def value(self) -> 'str|None':
         values = self.get_values(Token.NAME, Token.ARGUMENT)
         if values and values[0].upper() != 'NONE':
             return values[0]
         return None
 
 
-class MultiValue(Statement):
+class MultiValue(Statement, ABC):
 
     @property
-    def values(self):
+    def values(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
 
-class Fixture(Statement):
+class Fixture(Statement, ABC):
 
     @property
-    def name(self):
-        return self.get_value(Token.NAME)
+    def name(self) -> str:
+        return self.get_value(Token.NAME, '')
 
     @property
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
 
 @Statement.register
 class SectionHeader(Statement):
     handles_types = (Token.SETTING_HEADER, Token.VARIABLE_HEADER,
                      Token.TESTCASE_HEADER, Token.TASK_HEADER,
                      Token.KEYWORD_HEADER, Token.COMMENT_HEADER,
                      Token.INVALID_HEADER)
 
     @classmethod
-    def from_params(cls, type, name=None, eol=EOL):
+    def from_params(cls, type: str, name: 'str|None' = None,
+                    eol: str = EOL) -> 'SectionHeader':
         if not name:
             names = ('Settings', 'Variables', 'Test Cases', 'Tasks',
                      'Keywords', 'Comments')
             name = dict(zip(cls.handles_types, names))[type]
-        if not name.startswith('*'):
-            name = f'*** {name} ***'
+        name = cast(str, name)
+        header = f'*** {name} ***' if not name.startswith('*') else name
         return cls([
-            Token(type, name),
-            Token('EOL', '\n')
+            Token(type, header),
+            Token(Token.EOL, eol)
         ])
 
     @property
-    def type(self):
+    def type(self) -> str:
         token = self.get_token(*self.handles_types)
-        return token.type
+        return token.type    # type: ignore
 
     @property
-    def name(self):
+    def name(self) -> str:
         token = self.get_token(*self.handles_types)
-        return normalize_whitespace(token.value).strip('* ')
+        return normalize_whitespace(token.value).strip('* ') if token else ''
 
 
 @Statement.register
 class LibraryImport(Statement):
     type = Token.LIBRARY
 
     @classmethod
-    def from_params(cls, name, args=(), alias=None, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (), alias: 'str|None' = None,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'LibraryImport':
         tokens = [Token(Token.LIBRARY, 'Library'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         if alias is not None:
@@ -267,76 +347,79 @@
                            Token(Token.WITH_NAME),
                            Token(Token.SEPARATOR, separator),
                            Token(Token.NAME, alias)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def name(self):
-        return self.get_value(Token.NAME)
+    def name(self) -> str:
+        return self.get_value(Token.NAME, '')
 
     @property
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
     @property
-    def alias(self):
-        with_name = self.get_token(Token.WITH_NAME)
-        return self.get_tokens(Token.NAME)[-1].value if with_name else None
+    def alias(self) -> 'str|None':
+        separator = self.get_token(Token.WITH_NAME)
+        return self.get_tokens(Token.NAME)[-1].value if separator else None
 
 
 @Statement.register
 class ResourceImport(Statement):
     type = Token.RESOURCE
 
     @classmethod
-    def from_params(cls, name, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'ResourceImport':
         return cls([
             Token(Token.RESOURCE, 'Resource'),
             Token(Token.SEPARATOR, separator),
             Token(Token.NAME, name),
             Token(Token.EOL, eol)
         ])
 
     @property
-    def name(self):
-        return self.get_value(Token.NAME)
+    def name(self) -> str:
+        return self.get_value(Token.NAME, '')
 
 
 @Statement.register
 class VariablesImport(Statement):
     type = Token.VARIABLES
 
     @classmethod
-    def from_params(cls, name, args=(), separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'VariablesImport':
         tokens = [Token(Token.VARIABLES, 'Variables'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def name(self):
-        return self.get_value(Token.NAME)
+    def name(self) -> str:
+        return self.get_value(Token.NAME, '')
 
     @property
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
 
 @Statement.register
 class Documentation(DocumentationOrMetadata):
     type = Token.DOCUMENTATION
 
     @classmethod
-    def from_params(cls, value, indent=FOUR_SPACES, separator=FOUR_SPACES,
-                    eol=EOL, settings_section=True):
+    def from_params(cls, value: str, indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL,
+                    settings_section: bool = True) -> 'Documentation':
         if settings_section:
             tokens = [Token(Token.DOCUMENTATION, 'Documentation'),
                       Token(Token.SEPARATOR, separator)]
         else:
             tokens = [Token(Token.SEPARATOR, indent),
                       Token(Token.DOCUMENTATION, '[Documentation]'),
                       Token(Token.SEPARATOR, separator)]
@@ -346,31 +429,27 @@
             tokens.extend([Token(Token.ARGUMENT, doc_lines[0]),
                            Token(Token.EOL, eol)])
         for line in doc_lines[1:]:
             if not settings_section:
                 tokens.append(Token(Token.SEPARATOR, indent))
             tokens.append(Token(Token.CONTINUATION))
             if line:
-                tokens.extend([Token(Token.SEPARATOR, multiline_separator),
-                               Token(Token.ARGUMENT, line)])
-            tokens.append(Token(Token.EOL, eol))
+                tokens.append(Token(Token.SEPARATOR, multiline_separator))
+            tokens.extend([Token(Token.ARGUMENT, line),
+                           Token(Token.EOL, eol)])
         return cls(tokens)
 
-    @property
-    def value(self):
-        tokens = self.get_tokens(Token.ARGUMENT)
-        return self._join_value(tokens)
-
 
 @Statement.register
 class Metadata(DocumentationOrMetadata):
     type = Token.METADATA
 
     @classmethod
-    def from_params(cls, name, value, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, value: str, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'Metadata':
         tokens = [Token(Token.METADATA, 'Metadata'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         metadata_lines = value.splitlines()
         if metadata_lines:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, metadata_lines[0]),
@@ -379,71 +458,85 @@
             tokens.extend([Token(Token.CONTINUATION),
                            Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, line),
                            Token(Token.EOL, eol)])
         return cls(tokens)
 
     @property
-    def name(self):
-        return self.get_value(Token.NAME)
-
-    @property
-    def value(self):
-        tokens = self.get_tokens(Token.ARGUMENT)
-        return self._join_value(tokens)
+    def name(self) -> str:
+        return self.get_value(Token.NAME, '')
 
 
 @Statement.register
 class ForceTags(MultiValue):
     type = Token.FORCE_TAGS
 
     @classmethod
-    def from_params(cls, values, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, values: 'Sequence[str]', separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'ForceTags':
         tokens = [Token(Token.FORCE_TAGS, 'Force Tags')]
         for tag in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, tag)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
 
 @Statement.register
 class DefaultTags(MultiValue):
     type = Token.DEFAULT_TAGS
 
     @classmethod
-    def from_params(cls, values, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, values: 'Sequence[str]', separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'DefaultTags':
         tokens = [Token(Token.DEFAULT_TAGS, 'Default Tags')]
         for tag in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, tag)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
 
 @Statement.register
 class KeywordTags(MultiValue):
     type = Token.KEYWORD_TAGS
 
     @classmethod
-    def from_params(cls, values, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, values: 'Sequence[str]', separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'KeywordTags':
         tokens = [Token(Token.KEYWORD_TAGS, 'Keyword Tags')]
         for tag in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, tag)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
 
 @Statement.register
+class SuiteName(SingleValue):
+    type = Token.SUITE_NAME
+
+    @classmethod
+    def from_params(cls, value: str, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'SuiteName':
+        return cls([
+            Token(Token.SUITE_NAME, 'Name'),
+            Token(Token.SEPARATOR, separator),
+            Token(Token.NAME, value),
+            Token(Token.EOL, eol)
+        ])
+
+
+@Statement.register
 class SuiteSetup(Fixture):
     type = Token.SUITE_SETUP
 
     @classmethod
-    def from_params(cls, name, args=(), separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'SuiteSetup':
         tokens = [Token(Token.SUITE_SETUP, 'Suite Setup'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
@@ -451,15 +544,16 @@
 
 
 @Statement.register
 class SuiteTeardown(Fixture):
     type = Token.SUITE_TEARDOWN
 
     @classmethod
-    def from_params(cls, name, args=(), separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'SuiteTeardown':
         tokens = [Token(Token.SUITE_TEARDOWN, 'Suite Teardown'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
@@ -467,15 +561,16 @@
 
 
 @Statement.register
 class TestSetup(Fixture):
     type = Token.TEST_SETUP
 
     @classmethod
-    def from_params(cls, name, args=(), separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'TestSetup':
         tokens = [Token(Token.TEST_SETUP, 'Test Setup'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
@@ -483,15 +578,16 @@
 
 
 @Statement.register
 class TestTeardown(Fixture):
     type = Token.TEST_TEARDOWN
 
     @classmethod
-    def from_params(cls, name, args=(), separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'TestTeardown':
         tokens = [Token(Token.TEST_TEARDOWN, 'Test Teardown'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
@@ -499,128 +595,135 @@
 
 
 @Statement.register
 class TestTemplate(SingleValue):
     type = Token.TEST_TEMPLATE
 
     @classmethod
-    def from_params(cls, value, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, value: str, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'TestTemplate':
         return cls([
             Token(Token.TEST_TEMPLATE, 'Test Template'),
             Token(Token.SEPARATOR, separator),
             Token(Token.NAME, value),
             Token(Token.EOL, eol)
         ])
 
 
 @Statement.register
 class TestTimeout(SingleValue):
     type = Token.TEST_TIMEOUT
 
     @classmethod
-    def from_params(cls, value, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, value: str, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'TestTimeout':
         return cls([
             Token(Token.TEST_TIMEOUT, 'Test Timeout'),
             Token(Token.SEPARATOR, separator),
             Token(Token.ARGUMENT, value),
             Token(Token.EOL, eol)
         ])
 
 
 @Statement.register
 class Variable(Statement):
     type = Token.VARIABLE
 
     @classmethod
-    def from_params(cls, name, value, separator=FOUR_SPACES, eol=EOL):
-        """``value`` can be given either as a string or as a list of strings."""
-        values = value if is_list_like(value) else [value]
+    def from_params(cls, name: str, value: 'str|Sequence[str]',
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'Variable':
+        values = [value] if isinstance(value, str) else value
         tokens = [Token(Token.VARIABLE, name)]
         for value in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, value)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def name(self):
-        name = self.get_value(Token.VARIABLE)
+    def name(self) -> str:
+        name = self.get_value(Token.VARIABLE, '')
         if name.endswith('='):
             return name[:-1].rstrip()
         return name
 
     @property
-    def value(self):
+    def value(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
     def validate(self, ctx: 'ValidationContext'):
         name = self.get_value(Token.VARIABLE)
         match = search_variable(name, ignore_errors=True)
-        if not match.is_assign(allow_assign_mark=True):
+        if not match.is_assign(allow_assign_mark=True, allow_nested=True):
             self.errors += (f"Invalid variable name '{name}'.",)
         if match.is_dict_assign(allow_assign_mark=True):
             self._validate_dict_items()
 
     def _validate_dict_items(self):
         for item in self.get_values(Token.ARGUMENT):
             if not self._is_valid_dict_item(item):
                 self.errors += (
                     f"Invalid dictionary variable item '{item}'. "
                     f"Items must use 'name=value' syntax or be dictionary "
                     f"variables themselves.",
                 )
 
-    def _is_valid_dict_item(self, item):
+    def _is_valid_dict_item(self, item: str) -> bool:
         name, value = split_from_equals(item)
         return value is not None or is_dict_variable(item)
 
 
 @Statement.register
 class TestCaseName(Statement):
     type = Token.TESTCASE_NAME
 
     @classmethod
-    def from_params(cls, name, eol=EOL):
+    def from_params(cls, name: str, eol: str = EOL) -> 'TestCaseName':
         tokens = [Token(Token.TESTCASE_NAME, name)]
         if eol:
             tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def name(self):
-        return self.get_value(Token.TESTCASE_NAME)
+    def name(self) -> str:
+        return self.get_value(Token.TESTCASE_NAME, '')
 
     def validate(self, ctx: 'ValidationContext'):
         if not self.name:
-            self.errors += ('Test name cannot be empty.',)
+            self.errors += (test_or_task('{Test} name cannot be empty.', ctx.tasks),)
 
 
 @Statement.register
 class KeywordName(Statement):
     type = Token.KEYWORD_NAME
 
     @classmethod
-    def from_params(cls, name, eol=EOL):
+    def from_params(cls, name: str, eol: str = EOL) -> 'KeywordName':
         tokens = [Token(Token.KEYWORD_NAME, name)]
         if eol:
             tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def name(self):
-        return self.get_value(Token.KEYWORD_NAME)
+    def name(self) -> str:
+        return self.get_value(Token.KEYWORD_NAME, '')
+
+    def validate(self, ctx: 'ValidationContext'):
+        if not self.name:
+            self.errors += ('User keyword name cannot be empty.',)
 
 
 @Statement.register
 class Setup(Fixture):
     type = Token.SETUP
 
     @classmethod
-    def from_params(cls, name, args=(), indent=FOUR_SPACES, separator=FOUR_SPACES,
-                    eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    indent: str = FOUR_SPACES, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'Setup':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.SETUP, '[Setup]'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
@@ -629,16 +732,17 @@
 
 
 @Statement.register
 class Teardown(Fixture):
     type = Token.TEARDOWN
 
     @classmethod
-    def from_params(cls, name, args=(), indent=FOUR_SPACES, separator=FOUR_SPACES,
-                    eol=EOL):
+    def from_params(cls, name: str, args: 'Sequence[str]' = (),
+                    indent: str = FOUR_SPACES, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'Teardown':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.TEARDOWN, '[Teardown]'),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.NAME, name)]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
@@ -647,70 +751,74 @@
 
 
 @Statement.register
 class Tags(MultiValue):
     type = Token.TAGS
 
     @classmethod
-    def from_params(cls, values, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, values: 'Sequence[str]', indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'Tags':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.TAGS, '[Tags]')]
         for tag in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, tag)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
 
 @Statement.register
 class Template(SingleValue):
     type = Token.TEMPLATE
 
     @classmethod
-    def from_params(cls, value, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, value: str, indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'Template':
         return cls([
             Token(Token.SEPARATOR, indent),
             Token(Token.TEMPLATE, '[Template]'),
             Token(Token.SEPARATOR, separator),
             Token(Token.NAME, value),
             Token(Token.EOL, eol)
         ])
 
 
 @Statement.register
 class Timeout(SingleValue):
     type = Token.TIMEOUT
 
     @classmethod
-    def from_params(cls, value, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, value: str, indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'Timeout':
         return cls([
             Token(Token.SEPARATOR, indent),
             Token(Token.TIMEOUT, '[Timeout]'),
             Token(Token.SEPARATOR, separator),
             Token(Token.ARGUMENT, value),
             Token(Token.EOL, eol)
         ])
 
 
 @Statement.register
 class Arguments(MultiValue):
     type = Token.ARGUMENTS
 
     @classmethod
-    def from_params(cls, args, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, args: 'Sequence[str]', indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'Arguments':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.ARGUMENTS, '[Arguments]')]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     def validate(self, ctx: 'ValidationContext'):
-        errors = []
+        errors: 'list[str]' = []
         UserKeywordArgumentParser(error_reporter=errors.append).parse(self.values)
         self.errors = tuple(errors)
 
 
 # TODO: Change Return to mean ReturnStatement in RF 7.0
 # - Rename current Return to ReturnSetting
 # - Rename current ReturnStatement to Return
@@ -727,15 +835,16 @@
     be renamed to ``Return`` in Robot Framework 7.0.
 
     Eventually ``[Return]`` and ``ReturnSetting`` will be removed altogether.
     """
     type = Token.RETURN
 
     @classmethod
-    def from_params(cls, args, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, args: 'Sequence[str]', indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'Return':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.RETURN, '[Return]')]
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
@@ -746,252 +855,274 @@
 
 
 @Statement.register
 class KeywordCall(Statement):
     type = Token.KEYWORD
 
     @classmethod
-    def from_params(cls, name, assign=(), args=(), indent=FOUR_SPACES,
-                    separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, name: str, assign: 'Sequence[str]' = (),
+                    args: 'Sequence[str]' = (), indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'KeywordCall':
         tokens = [Token(Token.SEPARATOR, indent)]
         for assignment in assign:
             tokens.extend([Token(Token.ASSIGN, assignment),
                            Token(Token.SEPARATOR, separator)])
         tokens.append(Token(Token.KEYWORD, name))
         for arg in args:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def keyword(self):
-        return self.get_value(Token.KEYWORD)
+    def keyword(self) -> str:
+        return self.get_value(Token.KEYWORD, '')
 
     @property
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
     @property
-    def assign(self):
+    def assign(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ASSIGN)
 
 
 @Statement.register
 class TemplateArguments(Statement):
     type = Token.ARGUMENT
 
     @classmethod
-    def from_params(cls, args, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, args: 'Sequence[str]', indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'TemplateArguments':
         tokens = []
         for index, arg in enumerate(args):
             tokens.extend([Token(Token.SEPARATOR, separator if index else indent),
                            Token(Token.ARGUMENT, arg)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.get_values(self.type)
 
 
 @Statement.register
 class ForHeader(Statement):
     type = Token.FOR
 
     @classmethod
-    def from_params(cls, variables, values, flavor='IN', indent=FOUR_SPACES,
-                    separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, variables: 'Sequence[str]', values: 'Sequence[str]',
+                    flavor: str = 'IN', indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'ForHeader':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.FOR),
                   Token(Token.SEPARATOR, separator)]
         for variable in variables:
             tokens.extend([Token(Token.VARIABLE, variable),
                            Token(Token.SEPARATOR, separator)])
         tokens.append(Token(Token.FOR_SEPARATOR, flavor))
         for value in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, value)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def variables(self):
+    def variables(self) -> 'tuple[str, ...]':
         return self.get_values(Token.VARIABLE)
 
     @property
-    def values(self):
+    def values(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
     @property
-    def flavor(self):
+    def flavor(self) -> 'str|None':
         separator = self.get_token(Token.FOR_SEPARATOR)
         return normalize_whitespace(separator.value) if separator else None
 
     @property
-    def start(self):
+    def start(self) -> 'str|None':
         return self.get_option('start') if self.flavor == 'IN ENUMERATE' else None
 
     @property
-    def mode(self):
+    def mode(self) -> 'str|None':
         return self.get_option('mode') if self.flavor == 'IN ZIP' else None
 
     @property
-    def fill(self):
+    def fill(self) -> 'str|None':
         return self.get_option('fill') if self.flavor == 'IN ZIP' else None
 
     def validate(self, ctx: 'ValidationContext'):
+        self._validate_options()
         if not self.variables:
             self._add_error('no loop variables')
         if not self.flavor:
             self._add_error("no 'IN' or other valid separator")
         else:
             for var in self.variables:
                 if not is_scalar_assign(var):
                     self._add_error(f"invalid loop variable '{var}'")
             if not self.values:
                 self._add_error('no loop values')
 
-    def _add_error(self, error):
+    def _add_error(self, error: str):
         self.errors += (f'FOR loop has {error}.',)
 
 
-class IfElseHeader(Statement):
+class IfElseHeader(Statement, ABC):
 
     @property
-    def condition(self):
-        return None
+    def condition(self) -> 'str|None':
+        values = self.get_values(Token.ARGUMENT)
+        return ', '.join(values) if values else None
 
     @property
-    def assign(self):
-        return None
+    def assign(self) -> 'tuple[str, ...]':
+        return self.get_values(Token.ASSIGN)
+
+    def validate(self, ctx: 'ValidationContext'):
+        conditions = self.get_tokens(Token.ARGUMENT)
+        if not conditions:
+            self.errors += (f'{self.type} must have a condition.',)
+        if len(conditions) > 1:
+            self.errors += (f'{self.type} cannot have more than one condition, '
+                            f'got {seq2str(c.value for c in conditions)}.',)
 
 
 @Statement.register
 class IfHeader(IfElseHeader):
     type = Token.IF
 
     @classmethod
-    def from_params(cls, condition, indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
-        tokens = [Token(Token.SEPARATOR, indent),
-                  Token(cls.type),
-                  Token(Token.SEPARATOR, separator),
-                  Token(Token.ARGUMENT, condition)]
-        if cls.type != Token.INLINE_IF:
-            tokens.append(Token(Token.EOL, eol))
-        return cls(tokens)
-
-    @property
-    def condition(self):
-        values = self.get_values(Token.ARGUMENT)
-        if len(values) != 1:
-            return ', '.join(values) if values else None
-        return values[0]
-
-    def validate(self, ctx: 'ValidationContext'):
-        conditions = len(self.get_tokens(Token.ARGUMENT))
-        if conditions == 0:
-            self.errors += (f'{self.type} must have a condition.',)
-        if conditions > 1:
-            self.errors += (f'{self.type} cannot have more than one condition.',)
+    def from_params(cls, condition: str, indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'IfHeader':
+        return cls([
+            Token(Token.SEPARATOR, indent),
+            Token(cls.type),
+            Token(Token.SEPARATOR, separator),
+            Token(Token.ARGUMENT, condition),
+            Token(Token.EOL, eol)
+        ])
 
 
 @Statement.register
-class InlineIfHeader(IfHeader):
+class InlineIfHeader(IfElseHeader):
     type = Token.INLINE_IF
 
-    @property
-    def assign(self):
-        return self.get_values(Token.ASSIGN)
+    @classmethod
+    def from_params(cls, condition: str, assign: 'Sequence[str]' = (),
+                    indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES) -> 'InlineIfHeader':
+        tokens = [Token(Token.SEPARATOR, indent)]
+        for assignment in assign:
+            tokens.extend([Token(Token.ASSIGN, assignment),
+                           Token(Token.SEPARATOR, separator)])
+        tokens.extend([Token(Token.INLINE_IF),
+                       Token(Token.SEPARATOR, separator),
+                       Token(Token.ARGUMENT, condition)])
+        return cls(tokens)
 
 
 @Statement.register
-class ElseIfHeader(IfHeader):
+class ElseIfHeader(IfElseHeader):
     type = Token.ELSE_IF
 
+    @classmethod
+    def from_params(cls, condition: str, indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'ElseIfHeader':
+        return cls([
+            Token(Token.SEPARATOR, indent),
+            Token(Token.ELSE_IF),
+            Token(Token.SEPARATOR, separator),
+            Token(Token.ARGUMENT, condition),
+            Token(Token.EOL, eol)
+        ])
+
 
 @Statement.register
 class ElseHeader(IfElseHeader):
     type = Token.ELSE
 
     @classmethod
-    def from_params(cls, indent=FOUR_SPACES, eol=EOL):
+    def from_params(cls, indent: str = FOUR_SPACES, eol: str = EOL) -> 'ElseHeader':
         return cls([
             Token(Token.SEPARATOR, indent),
             Token(Token.ELSE),
             Token(Token.EOL, eol)
         ])
 
     def validate(self, ctx: 'ValidationContext'):
         if self.get_tokens(Token.ARGUMENT):
             values = self.get_values(Token.ARGUMENT)
             self.errors += (f'ELSE does not accept arguments, got {seq2str(values)}.',)
 
 
-class NoArgumentHeader(Statement):
+class NoArgumentHeader(Statement, ABC):
 
     @classmethod
-    def from_params(cls, indent=FOUR_SPACES, eol=EOL):
+    def from_params(cls, indent: str = FOUR_SPACES, eol: str = EOL):
         return cls([
             Token(Token.SEPARATOR, indent),
             Token(cls.type),
             Token(Token.EOL, eol)
         ])
 
     def validate(self, ctx: 'ValidationContext'):
         if self.get_tokens(Token.ARGUMENT):
             self.errors += (f'{self.type} does not accept arguments, got '
                             f'{seq2str(self.values)}.',)
 
     @property
-    def values(self):
+    def values(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
 
 @Statement.register
 class TryHeader(NoArgumentHeader):
     type = Token.TRY
 
 
 @Statement.register
 class ExceptHeader(Statement):
     type = Token.EXCEPT
 
     @classmethod
-    def from_params(cls, patterns=(), type=None, variable=None, indent=FOUR_SPACES,
-                    separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, patterns: 'Sequence[str]' = (), type: 'str|None' = None,
+                    variable: 'str|None' = None, indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'ExceptHeader':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.EXCEPT)]
         for pattern in patterns:
             tokens.extend([Token(Token.SEPARATOR, separator),
-                           Token(Token.ARGUMENT, pattern)]),
+                           Token(Token.ARGUMENT, pattern)])
         if type:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.OPTION, f'type={type}')])
         if variable:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.AS),
                            Token(Token.SEPARATOR, separator),
                            Token(Token.VARIABLE, variable)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def patterns(self):
+    def patterns(self) -> 'tuple[str, ...]':
         return self.get_values(Token.ARGUMENT)
 
     @property
-    def pattern_type(self):
+    def pattern_type(self) -> 'str|None':
         return self.get_option('type')
 
     @property
-    def variable(self):
+    def variable(self) -> 'str|None':
         return self.get_value(Token.VARIABLE)
 
     def validate(self, ctx: 'ValidationContext'):
+        self._validate_options()
         as_token = self.get_token(Token.AS)
         if as_token:
             variables = self.get_tokens(Token.VARIABLE)
             if not variables:
                 self.errors += ("EXCEPT's AS requires variable.",)
             elif len(variables) > 1:
                 self.errors += ("EXCEPT's AS accepts only one variable.",)
@@ -1010,55 +1141,74 @@
 
 
 @Statement.register
 class WhileHeader(Statement):
     type = Token.WHILE
 
     @classmethod
-    def from_params(cls, condition, limit=None, indent=FOUR_SPACES,
-                    separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, condition: str, limit: 'str|None' = None,
+                    on_limit: 'str|None ' = None, on_limit_message: 'str|None' = None,
+                    indent: str = FOUR_SPACES, separator: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'WhileHeader':
         tokens = [Token(Token.SEPARATOR, indent),
-                  Token(cls.type),
+                  Token(Token.WHILE),
                   Token(Token.SEPARATOR, separator),
                   Token(Token.ARGUMENT, condition)]
         if limit:
             tokens.extend([Token(Token.SEPARATOR, indent),
                            Token(Token.OPTION, f'limit={limit}')])
+        if on_limit:
+            tokens.extend([Token(Token.SEPARATOR, indent),
+                           Token(Token.OPTION, f'on_limit={on_limit}')])
+        if on_limit_message:
+            tokens.extend([Token(Token.SEPARATOR, indent),
+                           Token(Token.OPTION, f'on_limit_message={on_limit_message}')])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
 
     @property
-    def condition(self):
+    def condition(self) -> str:
         return ', '.join(self.get_values(Token.ARGUMENT))
 
     @property
-    def limit(self):
+    def limit(self) -> 'str|None':
         return self.get_option('limit')
 
+    @property
+    def on_limit(self) -> 'str|None':
+        return self.get_option('on_limit')
+
+    @property
+    def on_limit_message(self) -> 'str|None':
+        return self.get_option('on_limit_message')
+
     def validate(self, ctx: 'ValidationContext'):
-        values = self.get_values(Token.ARGUMENT)
-        if len(values) == 0:
-            self.errors += ('WHILE must have a condition.',)
-        if len(values) == 2:
-            self.errors += (f"Second WHILE loop argument must be 'limit', "
-                            f"got '{values[1]}'.",)
-        if len(values) > 2:
-            self.errors += ('WHILE cannot have more than one condition.',)
+        conditions = self.get_tokens(Token.ARGUMENT)
+        if len(conditions) > 1:
+            self._add_error(f'cannot have more than one condition, got '
+                            f'{seq2str(c.value for c in conditions)}')
+        if self.on_limit and not self.limit:
+            self._add_error("'on_limit' option cannot be used without 'limit'")
+        self._validate_options()
+
+    def _add_error(self, error: str):
+        self.errors += (f'WHILE loop {error}.',)
 
 
 @Statement.register
 class ReturnStatement(Statement):
     type = Token.RETURN_STATEMENT
 
     @property
     def values(self):
         return self.get_values(Token.ARGUMENT)
 
     @classmethod
-    def from_params(cls, values=(), indent=FOUR_SPACES, separator=FOUR_SPACES, eol=EOL):
+    def from_params(cls, values: 'Sequence[str]' = (), indent: str = FOUR_SPACES,
+                    separator: str = FOUR_SPACES, eol: str = EOL) -> 'ReturnStatement':
         tokens = [Token(Token.SEPARATOR, indent),
                   Token(Token.RETURN_STATEMENT)]
         for value in values:
             tokens.extend([Token(Token.SEPARATOR, separator),
                            Token(Token.ARGUMENT, value)])
         tokens.append(Token(Token.EOL, eol))
         return cls(tokens)
@@ -1066,15 +1216,15 @@
     def validate(self, ctx: 'ValidationContext'):
         if not ctx.in_keyword:
             self.errors += ('RETURN can only be used inside a user keyword.',)
         if ctx.in_finally:
             self.errors += ('RETURN cannot be used in FINALLY branch.',)
 
 
-class LoopControl(NoArgumentHeader):
+class LoopControl(NoArgumentHeader, ABC):
 
     def validate(self, ctx: 'ValidationContext'):
         super().validate(ctx)
         if not ctx.in_loop:
             self.errors += (f'{self.type} can only be used inside a loop.',)
         if ctx.in_finally:
             self.errors += (f'{self.type} cannot be used in FINALLY branch.',)
@@ -1091,62 +1241,72 @@
 
 
 @Statement.register
 class Comment(Statement):
     type = Token.COMMENT
 
     @classmethod
-    def from_params(cls, comment, indent=FOUR_SPACES, eol=EOL):
+    def from_params(cls, comment: str, indent: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'Comment':
         return cls([
             Token(Token.SEPARATOR, indent),
             Token(Token.COMMENT, comment),
             Token(Token.EOL, eol)
         ])
 
 
 @Statement.register
 class Config(Statement):
     type = Token.CONFIG
 
     @classmethod
-    def from_params(cls, config, eol=EOL):
+    def from_params(cls, config: str, eol: str = EOL) -> 'Config':
         return cls([
             Token(Token.CONFIG, config),
             Token(Token.EOL, eol)
         ])
 
     @property
-    def language(self):
+    def language(self) -> 'Language|None':
         value = self.get_value(Token.CONFIG)
         return Language.from_name(value[len('language:'):]) if value else None
 
 
 @Statement.register
 class Error(Statement):
     type = Token.ERROR
-    _errors = ()
+    _errors: 'tuple[str, ...]' = ()
+
+    @classmethod
+    def from_params(cls, error: str, value: str = '', indent: str = FOUR_SPACES,
+                    eol: str = EOL) -> 'Error':
+        return cls([
+            Token(Token.SEPARATOR, indent),
+            Token(Token.ERROR, value, error=error),
+            Token(Token.EOL, eol)
+        ])
 
     @property
-    def values(self):
-        return [t.value for t in self.data_tokens]
+    def values(self) -> 'list[str]':
+        return [token.value for token in self.data_tokens]
 
     @property
-    def errors(self):
+    def errors(self) -> 'tuple[str, ...]':
         """Errors got from the underlying ``ERROR``token.
 
         Errors can be set also explicitly. When accessing errors, they are returned
         along with errors got from tokens.
         """
         tokens = self.get_tokens(Token.ERROR)
-        return tuple(t.error for t in tokens) + self._errors
+        return tuple(t.error or '' for t in tokens) + self._errors
 
     @errors.setter
-    def errors(self, errors):
+    def errors(self, errors: 'Sequence[str]'):
         self._errors = tuple(errors)
 
 
 class EmptyLine(Statement):
     type = Token.EOL
 
     @classmethod
-    def from_params(cls, eol=EOL):
+    def from_params(cls, eol: str = EOL):
         return cls([Token(Token.EOL, eol)])
```

## Comparing `robotframework-6.1a1/src/robot/parsing/parser/blockparsers.py` & `robotframework-6.1b1/src/robot/parsing/parser/fileparser.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,124 +9,111 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from ..lexer import Token
-from ..model import TestCase, Keyword, For, If, Try, While
-
+from pathlib import Path
 
-class Parser:
-    """Base class for parsers."""
+from robot.utils import Source
 
-    def __init__(self, model):
-        self.model = model
+from ..lexer import Token
+from ..model import (CommentSection, File, ImplicitCommentSection, InvalidSection,
+                     Keyword, KeywordSection, Section, SettingSection, Statement,
+                     TestCase, TestCaseSection, VariableSection)
+from .blockparsers import KeywordParser, Parser, TestCaseParser
+
+
+class FileParser(Parser):
+    model: File
+
+    def __init__(self, source: 'Source|None' = None):
+        super().__init__(File(source=self._get_path(source)))
+        self.parsers: 'dict[str, type[SectionParser]]' = {
+            Token.SETTING_HEADER: SettingSectionParser,
+            Token.VARIABLE_HEADER: VariableSectionParser,
+            Token.TESTCASE_HEADER: TestCaseSectionParser,
+            Token.TASK_HEADER: TestCaseSectionParser,
+            Token.KEYWORD_HEADER: KeywordSectionParser,
+            Token.COMMENT_HEADER: CommentSectionParser,
+            Token.INVALID_HEADER: InvalidSectionParser,
+            Token.CONFIG: ImplicitCommentSectionParser,
+            Token.COMMENT: ImplicitCommentSectionParser,
+            Token.ERROR: ImplicitCommentSectionParser,
+            Token.EOL: ImplicitCommentSectionParser
+        }
 
-    def handles(self, statement):
-        raise NotImplementedError
+    def _get_path(self, source: 'Source|None') -> 'Path|None':
+        if not source:
+            return None
+        if isinstance(source, str) and '\n' not in source:
+            source = Path(source)
+        try:
+            if isinstance(source, Path) and source.is_file():
+                return source
+        except OSError:    # Can happen on Windows w/ Python < 3.10.
+            pass
+        return None
 
-    def parse(self, statement):
-        raise NotImplementedError
+    def handles(self, statement: Statement) -> bool:
+        return True
 
+    def parse(self, statement: Statement) -> 'SectionParser':
+        parser_class = self.parsers[statement.type]
+        model_class: 'type[Section]' = parser_class.__annotations__['model']
+        parser = parser_class(model_class(statement))
+        self.model.sections.append(parser.model)
+        return parser
 
-class BlockParser(Parser):
-    unhandled_tokens = Token.HEADER_TOKENS | frozenset((Token.TESTCASE_NAME,
-                                                        Token.KEYWORD_NAME))
 
-    def __init__(self, model):
-        Parser.__init__(self, model)
-        self.nested_parsers = {
-            Token.FOR: ForParser,
-            Token.IF: IfParser,
-            Token.INLINE_IF: IfParser,
-            Token.TRY: TryParser,
-            Token.WHILE: WhileParser
-        }
+class SectionParser(Parser):
+    model: Section
 
-    def handles(self, statement):
-        return statement.type not in self.unhandled_tokens
+    def handles(self, statement: Statement) -> bool:
+        return statement.type not in Token.HEADER_TOKENS
 
-    def parse(self, statement):
-        parser_class = self.nested_parsers.get(statement.type)
-        if parser_class:
-            parser = parser_class(statement)
-            self.model.body.append(parser.model)
-            return parser
+    def parse(self, statement: Statement) -> 'Parser|None':
         self.model.body.append(statement)
         return None
 
 
-class TestCaseParser(BlockParser):
+class SettingSectionParser(SectionParser):
+    model: SettingSection
 
-    def __init__(self, header):
-        BlockParser.__init__(self, TestCase(header))
 
+class VariableSectionParser(SectionParser):
+    model: VariableSection
 
-class KeywordParser(BlockParser):
 
-    def __init__(self, header):
-        BlockParser.__init__(self, Keyword(header))
+class CommentSectionParser(SectionParser):
+    model: CommentSection
 
 
-class NestedBlockParser(BlockParser):
-
-    def handles(self, statement):
-        return BlockParser.handles(self, statement) and \
-               not getattr(self.model, 'end', False)
-
-    def parse(self, statement):
-        if statement.type == Token.END:
-            self.model.end = statement
-            return None
-        return BlockParser.parse(self, statement)
+class ImplicitCommentSectionParser(SectionParser):
+    model: ImplicitCommentSection
 
 
-class ForParser(NestedBlockParser):
+class InvalidSectionParser(SectionParser):
+    model: InvalidSection
 
-    def __init__(self, header):
-        NestedBlockParser.__init__(self, For(header))
 
+class TestCaseSectionParser(SectionParser):
+    model: TestCaseSection
 
-class IfParser(NestedBlockParser):
-
-    def __init__(self, header, handle_end=True):
-        super().__init__(If(header))
-        self.handle_end = handle_end
-
-    def parse(self, statement):
-        if statement.type in (Token.ELSE_IF, Token.ELSE):
-            parser = IfParser(statement, handle_end=False)
-            self.model.orelse = parser.model
+    def parse(self, statement: Statement) -> 'Parser|None':
+        if statement.type == Token.TESTCASE_NAME:
+            parser = TestCaseParser(TestCase(statement))
+            self.model.body.append(parser.model)
             return parser
-        return NestedBlockParser.parse(self, statement)
-
-    def handles(self, statement):
-        if statement.type == Token.END and not self.handle_end:
-            return False
-        return super().handles(statement)
-
+        return super().parse(statement)
 
-class TryParser(NestedBlockParser):
 
-    def __init__(self, header, handle_end=True):
-        super().__init__(Try(header))
-        self.handle_end = handle_end
+class KeywordSectionParser(SectionParser):
+    model: KeywordSection
 
-    def parse(self, statement):
-        if statement.type in (Token.EXCEPT, Token.ELSE, Token.FINALLY):
-            parser = TryParser(statement, handle_end=False)
-            self.model.next = parser.model
+    def parse(self, statement: Statement) -> 'Parser|None':
+        if statement.type == Token.KEYWORD_NAME:
+            parser = KeywordParser(Keyword(statement))
+            self.model.body.append(parser.model)
             return parser
         return super().parse(statement)
-
-    def handles(self, statement):
-        if statement.type == Token.END and not self.handle_end:
-            return False
-        return super().handles(statement)
-
-
-class WhileParser(NestedBlockParser):
-
-    def __init__(self, header):
-        super().__init__(While(header))
```

## Comparing `robotframework-6.1a1/src/robot/parsing/parser/parser.py` & `robotframework-6.1b1/src/robot/parsing/parser/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,29 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from ..lexer import Token, get_tokens, get_resource_tokens, get_init_tokens
-from ..model import Statement, ModelVisitor
+from typing import Callable, Iterator
 
+from robot.conf import LanguagesLike
+from robot.utils import Source
+
+from ..lexer import get_init_tokens, get_resource_tokens, get_tokens, Token
+from ..model import File, Config, ModelVisitor, Statement
+
+from .blockparsers import Parser
 from .fileparser import FileParser
 
 
-def get_model(source, data_only=False, curdir=None, lang=None):
-    """Parses the given source to a model represented as an AST.
+def get_model(source: Source, data_only: bool = False, curdir: 'str|None' = None,
+              lang: LanguagesLike = None) -> File:
+    """Parses the given source into a model represented as an AST.
 
     How to use the model is explained more thoroughly in the general
     documentation of the :mod:`robot.parsing` module.
 
     :param source: The source where to read the data. Can be a path to
         a source file as a string or as ``pathlib.Path`` object, an already
         opened file object, or Unicode text containing the date directly.
@@ -32,84 +39,93 @@
     :param data_only: When ``False`` (default), returns all tokens. When set
         to ``True``, omits separators, comments, continuation markers, and
         other non-data tokens. Model like this cannot be saved back to
         file system.
     :param curdir: Directory where the source file exists. This path is used
         to set the value of the built-in ``${CURDIR}`` variable during parsing.
         When not given, the variable is left as-is. Should only be given
-        only if the model will be executed afterwards. If the model is saved
+        only if the model will be executed afterward. If the model is saved
         back to disk, resolving ``${CURDIR}`` is typically not a good idea.
     :param lang: Additional languages to be supported during parsing.
         Can be a string matching any of the supported language codes or names,
-        an initialized :class:`~robot.conf.languages.Language` subsclass,
+        an initialized :class:`~robot.conf.languages.Language` subclass,
         a list containing such strings or instances, or a
         :class:`~robot.conf.languages.Languages` instance.
 
     Use :func:`get_resource_model` or :func:`get_init_model` when parsing
     resource or suite initialization files, respectively.
     """
     return _get_model(get_tokens, source, data_only, curdir, lang)
 
 
-def get_resource_model(source, data_only=False, curdir=None, lang=None):
-    """Parses the given source to a resource file model.
+def get_resource_model(source: Source, data_only: bool = False,
+                       curdir: 'str|None' = None, lang: LanguagesLike = None) -> File:
+    """Parses the given source into a resource file model.
 
-    Otherwise same as :func:`get_model` but the source is considered to be
+    Same as :func:`get_model` otherwise, but the source is considered to be
     a resource file. This affects, for example, what settings are valid.
     """
     return _get_model(get_resource_tokens, source, data_only, curdir, lang)
 
 
-def get_init_model(source, data_only=False, curdir=None, lang=None):
-    """Parses the given source to a init file model.
+def get_init_model(source: Source, data_only: bool = False, curdir: 'str|None' = None,
+                   lang: LanguagesLike = None) -> File:
+    """Parses the given source into an init file model.
 
-    Otherwise same as :func:`get_model` but the source is considered to be
+    Same as :func:`get_model` otherwise, but the source is considered to be
     a suite initialization file. This affects, for example, what settings are
     valid.
     """
     return _get_model(get_init_tokens, source, data_only, curdir, lang)
 
 
-def _get_model(token_getter, source, data_only=False, curdir=None, lang=None):
+def _get_model(token_getter: Callable[..., Iterator[Token]], source: Source,
+               data_only: bool, curdir: 'str|None', lang: LanguagesLike):
     tokens = token_getter(source, data_only, lang=lang)
     statements = _tokens_to_statements(tokens, curdir)
     model = _statements_to_model(statements, source)
+    ConfigParser.parse(model)
     model.validate_model()
     return model
 
 
-def _tokens_to_statements(tokens, curdir=None):
+def _tokens_to_statements(tokens: Iterator[Token],
+                          curdir: 'str|None') -> Iterator[Statement]:
     statement = []
     EOS = Token.EOS
     for t in tokens:
         if curdir and '${CURDIR}' in t.value:
             t.value = t.value.replace('${CURDIR}', curdir)
         if t.type != EOS:
             statement.append(t)
         else:
             yield Statement.from_tokens(statement)
             statement = []
 
 
-def _statements_to_model(statements, source=None):
-    parser = FileParser(source=source)
-    model = parser.model
-    stack = [parser]
+def _statements_to_model(statements: Iterator[Statement], source: Source) -> File:
+    root = FileParser(source=source)
+    stack: 'list[Parser]' = [root]
     for statement in statements:
         while not stack[-1].handles(statement):
             stack.pop()
         parser = stack[-1].parse(statement)
         if parser:
             stack.append(parser)
-    # Implicit comment sections have no header.
-    if model.sections and model.sections[0].header is None:
-        SetLanguages(model).visit(model.sections[0])
-    return model
+    return root.model
+
 
+class ConfigParser(ModelVisitor):
 
-class SetLanguages(ModelVisitor):
+    def __init__(self, model: File):
+        self.model = model
 
-    def __init__(self, file):
-        self.file = file
+    @classmethod
+    def parse(cls, model: File):
+        # Only implicit comment sections can contain configs. They have no header.
+        if model.sections and model.sections[0].header is None:
+            cls(model).visit(model.sections[0])
 
-    def visit_Config(self, node):
-        self.file.languages += (node.language.code,)
+    def visit_Config(self, node: Config):
+        language = node.language
+        if language:
+            self.model.languages.append(language.code)
```

## Comparing `robotframework-6.1a1/src/robot/parsing/parser/__init__.py` & `robotframework-6.1b1/src/robot/parsing/parser/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/parsing/lexer/lexer.py` & `robotframework-6.1b1/src/robot/parsing/lexer/lexer.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,26 +9,31 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from collections.abc import Iterable, Iterator
 from itertools import chain
 
+from robot.conf import LanguagesLike
 from robot.errors import DataError
-from robot.utils import get_error_message, FileReader
+from robot.utils import get_error_message, FileReader, Source
 
 from .blocklexers import FileLexer
-from .context import InitFileContext, SuiteFileContext, ResourceFileContext
+from .context import (InitFileContext, LexingContext, SuiteFileContext,
+                      ResourceFileContext)
 from .tokenizer import Tokenizer
 from .tokens import EOS, END, Token
 
 
-def get_tokens(source, data_only=False, tokenize_variables=False, lang=None):
+def get_tokens(source: Source, data_only: bool = False,
+               tokenize_variables: bool = False,
+               lang: LanguagesLike = None) -> 'Iterator[Token]':
     """Parses the given source to tokens.
 
     :param source: The source where to read the data. Can be a path to
         a source file as a string or as ``pathlib.Path`` object, an already
         opened file object, or Unicode text containing the date directly.
         Source files must be UTF-8 encoded.
     :param data_only: When ``False`` (default), returns all tokens. When set
@@ -36,91 +41,96 @@
         other non-data tokens.
     :param tokenize_variables: When ``True``, possible variables in keyword
         arguments and elsewhere are tokenized. See the
         :meth:`~robot.parsing.lexer.tokens.Token.tokenize_variables`
         method for details.
     :param lang: Additional languages to be supported during parsing.
         Can be a string matching any of the supported language codes or names,
-        an initialized :class:`~robot.conf.languages.Language` subsclass,
+        an initialized :class:`~robot.conf.languages.Language` subclass,
         a list containing such strings or instances, or a
         :class:`~robot.conf.languages.Languages` instance.
 
     Returns a generator that yields :class:`~robot.parsing.lexer.tokens.Token`
     instances.
     """
     lexer = Lexer(SuiteFileContext(lang=lang), data_only, tokenize_variables)
     lexer.input(source)
     return lexer.get_tokens()
 
 
-def get_resource_tokens(source, data_only=False, tokenize_variables=False, lang=None):
+def get_resource_tokens(source: Source, data_only: bool = False,
+                        tokenize_variables: bool = False,
+                        lang: LanguagesLike = None) -> 'Iterator[Token]':
     """Parses the given source to resource file tokens.
 
     Same as :func:`get_tokens` otherwise, but the source is considered to be
     a resource file. This affects, for example, what settings are valid.
     """
     lexer = Lexer(ResourceFileContext(lang=lang), data_only, tokenize_variables)
     lexer.input(source)
     return lexer.get_tokens()
 
 
-def get_init_tokens(source, data_only=False, tokenize_variables=False, lang=None):
+def get_init_tokens(source: Source, data_only: bool = False,
+                    tokenize_variables: bool = False,
+                    lang: LanguagesLike = None) -> 'Iterator[Token]':
     """Parses the given source to init file tokens.
 
     Same as :func:`get_tokens` otherwise, but the source is considered to be
     a suite initialization file. This affects, for example, what settings are
     valid.
     """
     lexer = Lexer(InitFileContext(lang=lang), data_only, tokenize_variables)
     lexer.input(source)
     return lexer.get_tokens()
 
 
 class Lexer:
 
-    def __init__(self, ctx, data_only=False, tokenize_variables=False):
+    def __init__(self, ctx: LexingContext, data_only: bool = False,
+                 tokenize_variables: bool = False):
         self.lexer = FileLexer(ctx)
         self.data_only = data_only
         self.tokenize_variables = tokenize_variables
-        self.statements = []
+        self.statements: 'list[list[Token]]' = []
 
-    def input(self, source):
-        for statement in Tokenizer().tokenize(self._read(source),
-                                              self.data_only):
+    def input(self, source: Source):
+        for statement in Tokenizer().tokenize(self._read(source), self.data_only):
             # Store all tokens but pass only data tokens to lexer.
             self.statements.append(statement)
             if self.data_only:
                 data = statement[:]
             else:
                 # Separators, comments, etc. already have type, data doesn't.
                 data = [t for t in statement if t.type is None]
             if data:
                 self.lexer.input(data)
 
-    def _read(self, source):
+    def _read(self, source: Source) -> str:
         try:
             with FileReader(source, accept_text=True) as reader:
                 return reader.read()
         except Exception:
             raise DataError(get_error_message())
 
-    def get_tokens(self):
+    def get_tokens(self) -> 'Iterator[Token]':
         self.lexer.lex()
-        statements = self.statements
-        if not self.data_only:
+        if self.data_only:
+            statements = self.statements
+        else:
             statements = chain.from_iterable(
-                self._split_trailing_commented_and_empty_lines(s)
-                for s in statements
+                self._split_trailing_commented_and_empty_lines(stmt)
+                for stmt in self.statements
             )
         tokens = self._get_tokens(statements)
         if self.tokenize_variables:
             tokens = self._tokenize_variables(tokens)
         return tokens
 
-    def _get_tokens(self, statements):
+    def _get_tokens(self, statements: 'Iterable[list[Token]]') -> 'Iterator[Token]':
         if self.data_only:
             ignored_types = {None, Token.COMMENT_HEADER, Token.COMMENT}
         else:
             ignored_types = {None}
         inline_if_type = Token.INLINE_IF
         for statement in statements:
             last = None
@@ -133,50 +143,51 @@
                     yield EOS.from_token(token, before=True)
                 yield token
                 if token._add_eos_after:
                     yield EOS.from_token(token)
                 if token_type == inline_if_type:
                     inline_if = True
                 last = token
-            if last and not last._add_eos_after:
-                yield EOS.from_token(last)
-            if inline_if:
-                yield END.from_token(last, virtual=True)
-                yield EOS.from_token(last)
+            if last:
+                if not last._add_eos_after:
+                    yield EOS.from_token(last)
+                if inline_if:
+                    yield END.from_token(last, virtual=True)
+                    yield EOS.from_token(last)
 
-    def _split_trailing_commented_and_empty_lines(self, statement):
+    def _split_trailing_commented_and_empty_lines(self, statement: 'list[Token]') \
+            -> 'list[list[Token]]':
         lines = self._split_to_lines(statement)
         commented_or_empty = []
         for line in reversed(lines):
             if not self._is_commented_or_empty(line):
                 break
             commented_or_empty.append(line)
         if not commented_or_empty:
             return [statement]
         lines = lines[:-len(commented_or_empty)]
         statement = list(chain.from_iterable(lines))
         return [statement] + list(reversed(commented_or_empty))
 
-    def _split_to_lines(self, statement):
+    def _split_to_lines(self, statement: 'list[Token]') -> 'list[list[Token]]':
         lines = []
         current = []
         for token in statement:
             current.append(token)
             if token.type == Token.EOL:
                 lines.append(current)
                 current = []
         if current:
             lines.append(current)
         return lines
 
-    def _is_commented_or_empty(self, line):
+    def _is_commented_or_empty(self, line: 'list[Token]') -> bool:
         separator_or_ignore = (Token.SEPARATOR, None)
         comment_or_eol = (Token.COMMENT, Token.EOL)
         for token in line:
             if token.type not in separator_or_ignore:
                 return token.type in comment_or_eol
         return False
 
-    def _tokenize_variables(self, tokens):
+    def _tokenize_variables(self, tokens: 'Iterator[Token]') -> 'Iterator[Token]':
         for token in tokens:
-            for t in token.tokenize_variables():
-                yield t
+            yield from token.tokenize_variables()
```

## Comparing `robotframework-6.1a1/src/robot/parsing/lexer/context.py` & `robotframework-6.1b1/src/robot/parsing/lexer/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,135 +9,137 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from robot.conf import Languages
+from robot.conf import Languages, LanguageLike, LanguagesLike
 from robot.utils import normalize_whitespace
 
-from .settings import (InitFileSettings, SuiteFileSettings, ResourceFileSettings,
-                       TestCaseSettings, KeywordSettings)
-from .tokens import Token
+from .settings import (InitFileSettings, FileSettings, Settings, SuiteFileSettings,
+                       ResourceFileSettings, TestCaseSettings, KeywordSettings)
+from .tokens import StatementTokens, Token
 
 
 class LexingContext:
-    settings_class = None
 
-    def __init__(self, settings=None, lang=None):
-        if not settings:
-            self.languages = lang if isinstance(lang, Languages) else Languages(lang)
-            self.settings = self.settings_class(self.languages)
-        else:
-            self.languages = settings.languages
-            self.settings = settings
+    def __init__(self, settings: Settings, languages: Languages):
+        self.settings = settings
+        self.languages = languages
 
-    def lex_setting(self, statement):
+    def lex_setting(self, statement: StatementTokens):
         self.settings.lex(statement)
 
 
 class FileContext(LexingContext):
+    settings: FileSettings
 
-    def __init__(self, settings=None, lang=None):
-        super().__init__(settings, lang)
+    def __init__(self, lang: LanguagesLike = None):
+        languages = lang if isinstance(lang, Languages) else Languages(lang)
+        settings_class: 'type[FileSettings]' = type(self).__annotations__['settings']
+        settings = settings_class(languages)
+        super().__init__(settings, languages)
 
-    def add_language(self, lang):
+    def add_language(self, lang: LanguageLike):
         self.languages.add_language(lang)
 
-    def keyword_context(self):
-        return KeywordContext(settings=KeywordSettings(self.languages))
+    def keyword_context(self) -> 'KeywordContext':
+        return KeywordContext(KeywordSettings(self.settings))
 
-    def setting_section(self, statement):
+    def setting_section(self, statement: StatementTokens) -> bool:
         return self._handles_section(statement, 'Settings')
 
-    def variable_section(self, statement):
+    def variable_section(self, statement: StatementTokens) -> bool:
         return self._handles_section(statement, 'Variables')
 
-    def test_case_section(self, statement):
+    def test_case_section(self, statement: StatementTokens) -> bool:
         return False
 
-    def task_section(self, statement):
+    def task_section(self, statement: StatementTokens) -> bool:
         return False
 
-    def keyword_section(self, statement):
+    def keyword_section(self, statement: StatementTokens) -> bool:
         return self._handles_section(statement, 'Keywords')
 
-    def comment_section(self, statement):
+    def comment_section(self, statement: StatementTokens) -> bool:
         return self._handles_section(statement, 'Comments')
 
-    def lex_invalid_section(self, statement):
-        message = self._get_invalid_section_error(statement[0].value)
-        statement[0].error = message
-        statement[0].type = Token.INVALID_HEADER
+    def lex_invalid_section(self, statement: StatementTokens):
+        header = statement[0]
+        header.type = Token.INVALID_HEADER
+        header.error = self._get_invalid_section_error(header.value)
         for token in statement[1:]:
             token.type = Token.COMMENT
 
-    def _get_invalid_section_error(self, header):
+    def _get_invalid_section_error(self, header: str) -> str:
         raise NotImplementedError
 
-    def _handles_section(self, statement, header):
+    def _handles_section(self, statement: StatementTokens, header: str) -> bool:
         marker = statement[0].value
-        return (marker and marker[0] == '*' and
-                self.languages.headers.get(self._normalize(marker)) == header)
+        return bool(marker and marker[0] == '*' and
+                    self.languages.headers.get(self._normalize(marker)) == header)
 
-    def _normalize(self, marker):
+    def _normalize(self, marker: str) -> str:
         return normalize_whitespace(marker).strip('* ').title()
 
 
 class SuiteFileContext(FileContext):
-    settings_class = SuiteFileSettings
+    settings: SuiteFileSettings
 
-    def test_case_context(self):
-        return TestCaseContext(settings=TestCaseSettings(self.settings, self.languages))
+    def test_case_context(self) -> 'TestCaseContext':
+        return TestCaseContext(TestCaseSettings(self.settings))
 
-    def test_case_section(self, statement):
+    def test_case_section(self, statement: StatementTokens) -> bool:
         return self._handles_section(statement, 'Test Cases')
 
-    def task_section(self, statement):
+    def task_section(self, statement: StatementTokens) -> bool:
         return self._handles_section(statement, 'Tasks')
 
-    def _get_invalid_section_error(self, header):
+    def _get_invalid_section_error(self, header: str) -> str:
         return (f"Unrecognized section header '{header}'. Valid sections: "
                 f"'Settings', 'Variables', 'Test Cases', 'Tasks', 'Keywords' "
                 f"and 'Comments'.")
 
 
 class ResourceFileContext(FileContext):
-    settings_class = ResourceFileSettings
+    settings: ResourceFileSettings
 
-    def _get_invalid_section_error(self, header):
+    def _get_invalid_section_error(self, header: str) -> str:
         name = self._normalize(header)
         if self.languages.headers.get(name) in ('Test Cases', 'Tasks'):
             return f"Resource file with '{name}' section is invalid."
         return (f"Unrecognized section header '{header}'. Valid sections: "
                 f"'Settings', 'Variables', 'Keywords' and 'Comments'.")
 
 
-
 class InitFileContext(FileContext):
-    settings_class = InitFileSettings
+    settings: InitFileSettings
 
-    def _get_invalid_section_error(self, header):
+    def _get_invalid_section_error(self, header: str) -> str:
         name = self._normalize(header)
         if self.languages.headers.get(name) in ('Test Cases', 'Tasks'):
             return f"'{name}' section is not allowed in suite initialization file."
         return (f"Unrecognized section header '{header}'. Valid sections: "
                 f"'Settings', 'Variables', 'Keywords' and 'Comments'.")
 
 
-class TestOrKeywordContext(LexingContext):
-
-    @property
-    def template_set(self):
-        return False
-
+class TestCaseContext(LexingContext):
+    settings: TestCaseSettings
 
-class TestCaseContext(TestOrKeywordContext):
+    def __init__(self, settings: TestCaseSettings):
+        super().__init__(settings, settings.languages)
 
     @property
-    def template_set(self):
+    def template_set(self) -> bool:
         return self.settings.template_set
 
 
-class KeywordContext(TestOrKeywordContext):
-    pass
+class KeywordContext(LexingContext):
+    settings: KeywordSettings
+
+    def __init__(self, settings: KeywordSettings):
+        super().__init__(settings, settings.languages)
+
+    @property
+    def template_set(self) -> bool:
+        return False
```

## Comparing `robotframework-6.1a1/src/robot/parsing/lexer/settings.py` & `robotframework-6.1b1/src/robot/parsing/lexer/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from abc import ABC, abstractmethod
+
+from robot.conf import Languages
 from robot.utils import normalize, normalize_whitespace, RecommendationFinder
 
-from .tokens import Token
+from .tokens import StatementTokens, Token
 
 
-class Settings:
-    names = ()
-    aliases = {}
+class Settings(ABC):
+    names: 'tuple[str, ...]' = ()
+    aliases: 'dict[str, str]' = {}
     multi_use = (
         'Metadata',
         'Library',
         'Resource',
         'Variables'
     )
     single_value = (
         'Resource',
         'Test Timeout',
         'Test Template',
         'Timeout',
-        'Template'
+        'Template',
+        'Name'
     )
     name_and_arguments = (
         'Metadata',
         'Suite Setup',
         'Suite Teardown',
         'Test Setup',
         'Test Teardown',
@@ -47,101 +51,108 @@
         'Resource',
         'Variables'
     )
     name_arguments_and_with_name = (
         'Library',
     )
 
-    def __init__(self, languages):
-        self.settings = {n: None for n in self.names}
+    def __init__(self, languages: Languages):
+        self.settings: 'dict[str, list[Token]|None]' = {n: None for n in self.names}
         self.languages = languages
 
-    def lex(self, statement):
-        setting = statement[0]
-        orig = self._format_name(setting.value)
+    def lex(self, statement: StatementTokens):
+        orig = self._format_name(statement[0].value)
         name = normalize_whitespace(orig).title()
         name = self.languages.settings.get(name, name)
         if name in self.aliases:
             name = self.aliases[name]
         try:
             self._validate(orig, name, statement)
         except ValueError as err:
-            self._lex_error(setting, statement[1:], err.args[0])
+            self._lex_error(statement, err.args[0])
         else:
-            self._lex_setting(setting, statement[1:], name)
+            self._lex_setting(statement, name)
 
-    def _format_name(self, name):
+    def _format_name(self, name: str) -> str:
         return name
 
-    def _validate(self, orig, name, statement):
+    def _validate(self, orig: str, name: str, statement: StatementTokens):
         if name not in self.settings:
             message = self._get_non_existing_setting_message(orig, name)
             raise ValueError(message)
         if self.settings[name] is not None and name not in self.multi_use:
             raise ValueError(f"Setting '{orig}' is allowed only once. "
                              f"Only the first value is used.")
         if name in self.single_value and len(statement) > 2:
             raise ValueError(f"Setting '{orig}' accepts only one value, "
                              f"got {len(statement)-1}.")
 
-    def _get_non_existing_setting_message(self, name, normalized):
-        if self._is_valid_somewhere(normalized):
+    def _get_non_existing_setting_message(self, name: str, normalized: str) -> str:
+        if self._is_valid_somewhere(normalized, Settings.__subclasses__()):
             return self._not_valid_here(name)
         return RecommendationFinder(normalize).find_and_format(
             name=normalized,
             candidates=tuple(self.settings) + tuple(self.aliases),
             message=f"Non-existing setting '{name}'."
         )
 
-    def _is_valid_somewhere(self, normalized):
-        for cls in Settings.__subclasses__():
-            if normalized in cls.names or normalized in cls.aliases:
+    def _is_valid_somewhere(self, name: str, classes: 'list[type[Settings]]') -> bool:
+        for cls in classes:
+            if (name in cls.names or name in cls.aliases
+                    or self._is_valid_somewhere(name, cls.__subclasses__())):
                 return True
         return False
 
-    def _not_valid_here(self, name):
+    @abstractmethod
+    def _not_valid_here(self, name: str) -> str:
         raise NotImplementedError
 
-    def _lex_error(self, setting, values, error):
-        setting.set_error(error)
-        for token in values:
+    def _lex_error(self, statement: StatementTokens, error: str):
+        statement[0].set_error(error)
+        for token in statement[1:]:
             token.type = Token.COMMENT
 
-    def _lex_setting(self, setting, values, name):
-        self.settings[name] = values
+    def _lex_setting(self, statement: StatementTokens, name: str):
         # TODO: Change token type from 'FORCE TAGS' to 'TEST TAGS' in RF 7.0.
-        setting.type = name.upper() if name != 'Test Tags' else 'FORCE TAGS'
+        statement[0].type = {'Test Tags': Token.FORCE_TAGS,
+                             'Name': Token.SUITE_NAME}.get(name, name.upper())
+        self.settings[name] = values = statement[1:]
         if name in self.name_and_arguments:
             self._lex_name_and_arguments(values)
         elif name in self.name_arguments_and_with_name:
             self._lex_name_arguments_and_with_name(values)
         else:
             self._lex_arguments(values)
 
-    def _lex_name_and_arguments(self, tokens):
+    def _lex_name_and_arguments(self, tokens: StatementTokens):
         if tokens:
             tokens[0].type = Token.NAME
-        self._lex_arguments(tokens[1:])
+            self._lex_arguments(tokens[1:])
 
-    def _lex_name_arguments_and_with_name(self, tokens):
+    def _lex_name_arguments_and_with_name(self, tokens: StatementTokens):
         self._lex_name_and_arguments(tokens)
         if len(tokens) > 1 and \
                 normalize_whitespace(tokens[-2].value) in ('WITH NAME', 'AS'):
             tokens[-2].type = Token.WITH_NAME
             tokens[-1].type = Token.NAME
 
-    def _lex_arguments(self, tokens):
+    def _lex_arguments(self, tokens: StatementTokens):
         for token in tokens:
             token.type = Token.ARGUMENT
 
 
-class SuiteFileSettings(Settings):
+class FileSettings(Settings, ABC):
+    pass
+
+
+class SuiteFileSettings(FileSettings):
     names = (
         'Documentation',
         'Metadata',
+        'Name',
         'Suite Setup',
         'Suite Teardown',
         'Test Setup',
         'Test Teardown',
         'Test Template',
         'Test Timeout',
         'Test Tags',
@@ -156,22 +167,23 @@
         'Task Tags': 'Test Tags',
         'Task Setup': 'Test Setup',
         'Task Teardown': 'Test Teardown',
         'Task Template': 'Test Template',
         'Task Timeout': 'Test Timeout',
     }
 
-    def _not_valid_here(self, name):
+    def _not_valid_here(self, name: str) -> str:
         return f"Setting '{name}' is not allowed in suite file."
 
 
-class InitFileSettings(Settings):
+class InitFileSettings(FileSettings):
     names = (
         'Documentation',
         'Metadata',
+        'Name',
         'Suite Setup',
         'Suite Teardown',
         'Test Setup',
         'Test Teardown',
         'Test Timeout',
         'Test Tags',
         'Keyword Tags',
@@ -183,76 +195,80 @@
         'Force Tags': 'Test Tags',
         'Task Tags': 'Test Tags',
         'Task Setup': 'Test Setup',
         'Task Teardown': 'Test Teardown',
         'Task Timeout': 'Test Timeout',
     }
 
-    def _not_valid_here(self, name):
+    def _not_valid_here(self, name: str) -> str:
         return f"Setting '{name}' is not allowed in suite initialization file."
 
 
-class ResourceFileSettings(Settings):
+class ResourceFileSettings(FileSettings):
     names = (
         'Documentation',
         'Keyword Tags',
         'Library',
         'Resource',
         'Variables'
     )
 
-    def _not_valid_here(self, name):
+    def _not_valid_here(self, name: str) -> str:
         return f"Setting '{name}' is not allowed in resource file."
 
 
 class TestCaseSettings(Settings):
     names = (
         'Documentation',
         'Tags',
         'Setup',
         'Teardown',
         'Template',
         'Timeout'
     )
 
-    def __init__(self, parent, languages):
-        super().__init__(languages)
+    def __init__(self, parent: SuiteFileSettings):
+        super().__init__(parent.languages)
         self.parent = parent
 
-    def _format_name(self, name):
+    def _format_name(self, name: str) -> str:
         return name[1:-1].strip()
 
     @property
-    def template_set(self):
+    def template_set(self) -> bool:
         template = self.settings['Template']
         if self._has_disabling_value(template):
             return False
         parent_template = self.parent.settings['Test Template']
         return self._has_value(template) or self._has_value(parent_template)
 
-    def _has_disabling_value(self, setting):
+    def _has_disabling_value(self, setting: 'StatementTokens|None') -> bool:
         if setting is None:
             return False
         return setting == [] or setting[0].value.upper() == 'NONE'
 
-    def _has_value(self, setting):
-        return setting and setting[0].value
+    def _has_value(self, setting: 'StatementTokens|None') -> bool:
+        return bool(setting and setting[0].value)
 
-    def _not_valid_here(self, name):
+    def _not_valid_here(self, name: str) -> str:
         return f"Setting '{name}' is not allowed with tests or tasks."
 
 
 class KeywordSettings(Settings):
     names = (
         'Documentation',
         'Arguments',
         'Teardown',
         'Timeout',
         'Tags',
         'Return'
     )
 
-    def _format_name(self, name):
+    def __init__(self, parent: FileSettings):
+        super().__init__(parent.languages)
+        self.parent = parent
+
+    def _format_name(self, name: str) -> str:
         return name[1:-1].strip()
 
-    def _not_valid_here(self, name):
+    def _not_valid_here(self, name: str) -> str:
         return f"Setting '{name}' is not allowed with user keywords."
```

## Comparing `robotframework-6.1a1/src/robot/parsing/lexer/tokens.py` & `robotframework-6.1b1/src/robot/parsing/lexer/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,51 +9,55 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from collections.abc import Iterator
+from typing import cast, List
+
 from robot.variables import VariableIterator
 
 
+# Type alias to ease typing elsewhere
+StatementTokens = List['Token']
+
+
 class Token:
     """Token representing piece of Robot Framework data.
 
     Each token has type, value, line number, column offset and end column
     offset in :attr:`type`, :attr:`value`, :attr:`lineno`, :attr:`col_offset`
     and :attr:`end_col_offset` attributes, respectively. Tokens representing
     error also have their error message in :attr:`error` attribute.
 
     Token types are declared as class attributes such as :attr:`SETTING_HEADER`
     and :attr:`EOL`. Values of these constants have changed slightly in Robot
-    Framework 4.0 and they may change again in the future. It is thus safer
+    Framework 4.0, and they may change again in the future. It is thus safer
     to use the constants, not their values, when types are needed. For example,
     use ``Token(Token.EOL)`` instead of ``Token('EOL')`` and
     ``token.type == Token.EOL`` instead of ``token.type == 'EOL'``.
 
-    If :attr:`value` is not given when :class:`Token` is initialized and
-    :attr:`type` is :attr:`IF`, :attr:`ELSE_IF`, :attr:`ELSE`, :attr:`FOR`,
-    :attr:`END`, :attr:`WITH_NAME` or :attr:`CONTINUATION`, the value is
-    automatically set to the correct marker value like ``'IF'`` or ``'ELSE IF'``.
-    If :attr:`type` is :attr:`EOL` in this case, the value is set to ``'\\n'``.
+    If :attr:`value` is not given and :attr:`type` is a special marker like
+    :attr:`IF` or `:attr:`EOL`, the value is set automatically.
     """
 
     SETTING_HEADER = 'SETTING HEADER'
     VARIABLE_HEADER = 'VARIABLE HEADER'
     TESTCASE_HEADER = 'TESTCASE HEADER'
     TASK_HEADER = 'TASK HEADER'
     KEYWORD_HEADER = 'KEYWORD HEADER'
     COMMENT_HEADER = 'COMMENT HEADER'
     INVALID_HEADER = 'INVALID HEADER'
     FATAL_INVALID_HEADER = 'FATAL INVALID HEADER'
 
     TESTCASE_NAME = 'TESTCASE NAME'
     KEYWORD_NAME = 'KEYWORD NAME'
-
+    SUITE_NAME = 'SUITE NAME'
     DOCUMENTATION = 'DOCUMENTATION'
     SUITE_SETUP = 'SUITE SETUP'
     SUITE_TEARDOWN = 'SUITE TEARDOWN'
     METADATA = 'METADATA'
     TEST_SETUP = 'TEST SETUP'
     TEST_TEARDOWN = 'TEST TEARDOWN'
     TEST_TEMPLATE = 'TEST TEMPLATE'
@@ -71,31 +75,33 @@
     TAGS = 'TAGS'
     ARGUMENTS = 'ARGUMENTS'
     # Use ´RETURN_SETTING` type instead of `RETURN`. `[Return]` is deprecated and
     # `RETURN` type will be used with `RETURN` statement in the future.
     RETURN = 'RETURN'
     RETURN_SETTING = RETURN
 
+    # TODO: Change WITH_NAME value to AS in RF 7.0. Remove WITH_NAME in RF 8.
+    WITH_NAME = 'WITH NAME'
+    AS = 'AS'
+
     NAME = 'NAME'
     VARIABLE = 'VARIABLE'
     ARGUMENT = 'ARGUMENT'
     ASSIGN = 'ASSIGN'
     KEYWORD = 'KEYWORD'
-    WITH_NAME = 'WITH NAME'
     FOR = 'FOR'
     FOR_SEPARATOR = 'FOR SEPARATOR'
     END = 'END'
     IF = 'IF'
     INLINE_IF = 'INLINE IF'
     ELSE_IF = 'ELSE IF'
     ELSE = 'ELSE'
     TRY = 'TRY'
     EXCEPT = 'EXCEPT'
     FINALLY = 'FINALLY'
-    AS = 'AS'
     WHILE = 'WHILE'
     RETURN_STATEMENT = 'RETURN STATEMENT'
     CONTINUE = 'CONTINUE'
     BREAK = 'BREAK'
     OPTION = 'OPTION'
 
     SEPARATOR = 'SEPARATOR'
@@ -114,14 +120,15 @@
         COMMENT,
         CONTINUATION,
         EOL,
         EOS
     ))
     SETTING_TOKENS = frozenset((
         DOCUMENTATION,
+        SUITE_NAME,
         SUITE_SETUP,
         SUITE_TEARDOWN,
         METADATA,
         TEST_SETUP,
         TEST_TEARDOWN,
         TEST_TEMPLATE,
         TEST_TIMEOUT,
@@ -150,118 +157,117 @@
     ))
     ALLOW_VARIABLES = frozenset((
         NAME,
         ARGUMENT,
         TESTCASE_NAME,
         KEYWORD_NAME
     ))
-
     __slots__ = ['type', 'value', 'lineno', 'col_offset', 'error',
                  '_add_eos_before', '_add_eos_after']
 
-    def __init__(self, type=None, value=None, lineno=-1, col_offset=-1, error=None):
+    def __init__(self, type: 'str|None' = None, value: 'str|None' = None,
+                 lineno: int = -1, col_offset: int = -1, error: 'str|None' = None):
         self.type = type
         if value is None:
             value = {
                 Token.IF: 'IF', Token.INLINE_IF: 'IF', Token.ELSE_IF: 'ELSE IF',
                 Token.ELSE: 'ELSE', Token.FOR: 'FOR', Token.WHILE: 'WHILE',
                 Token.TRY: 'TRY', Token.EXCEPT: 'EXCEPT', Token.FINALLY: 'FINALLY',
                 Token.END: 'END', Token.CONTINUE: 'CONTINUE', Token.BREAK: 'BREAK',
                 Token.RETURN_STATEMENT: 'RETURN', Token.CONTINUATION: '...',
                 Token.EOL: '\n', Token.WITH_NAME: 'WITH NAME', Token.AS: 'AS'
-            }.get(type, '')
-        self.value = value
+            }.get(type, '')    # type: ignore
+        self.value = cast(str, value)
         self.lineno = lineno
         self.col_offset = col_offset
         self.error = error
         # Used internally be lexer to indicate that EOS is needed before/after.
         self._add_eos_before = False
         self._add_eos_after = False
 
     @property
-    def end_col_offset(self):
+    def end_col_offset(self) -> int:
         if self.col_offset == -1:
             return -1
         return self.col_offset + len(self.value)
 
-    def set_error(self, error):
+    def set_error(self, error: str):
         self.type = Token.ERROR
         self.error = error
 
-    def tokenize_variables(self):
+    def tokenize_variables(self) -> 'Iterator[Token]':
         """Tokenizes possible variables in token value.
 
         Yields the token itself if the token does not allow variables (see
         :attr:`Token.ALLOW_VARIABLES`) or its value does not contain
-        variables. Otherwise yields variable tokens as well as tokens
+        variables. Otherwise, yields variable tokens as well as tokens
         before, after, or between variables so that they have the same
         type as the original token.
         """
         if self.type not in Token.ALLOW_VARIABLES:
             return self._tokenize_no_variables()
         variables = VariableIterator(self.value)
         if not variables:
             return self._tokenize_no_variables()
         return self._tokenize_variables(variables)
 
-    def _tokenize_no_variables(self):
+    def _tokenize_no_variables(self) -> 'Iterator[Token]':
         yield self
 
-    def _tokenize_variables(self, variables):
+    def _tokenize_variables(self, variables) -> 'Iterator[Token]':
         lineno = self.lineno
         col_offset = self.col_offset
         remaining = ''
         for before, variable, remaining in variables:
             if before:
                 yield Token(self.type, before, lineno, col_offset)
                 col_offset += len(before)
             yield Token(Token.VARIABLE, variable, lineno, col_offset)
             col_offset += len(variable)
         if remaining:
             yield Token(self.type, remaining, lineno, col_offset)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.value
 
-    def __repr__(self):
-        type_ = self.type.replace(' ', '_') if self.type else 'None'
-        error = '' if not self.error else ', %r' % self.error
-        return 'Token(%s, %r, %s, %s%s)' % (type_, self.value, self.lineno,
-                                            self.col_offset, error)
+    def __repr__(self) -> str:
+        typ = self.type.replace(' ', '_') if self.type else 'None'
+        error = '' if not self.error else f', {self.error!r}'
+        return f'Token({typ}, {self.value!r}, {self.lineno}, {self.col_offset}{error})'
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return (isinstance(other, Token)
                 and self.type == other.type
                 and self.value == other.value
                 and self.lineno == other.lineno
                 and self.col_offset == other.col_offset
                 and self.error == other.error)
 
 
 class EOS(Token):
     """Token representing end of a statement."""
     __slots__ = []
 
-    def __init__(self, lineno=-1, col_offset=-1):
-        Token.__init__(self, Token.EOS, '', lineno, col_offset)
+    def __init__(self, lineno: int = -1, col_offset: int = -1):
+        super().__init__(Token.EOS, '', lineno, col_offset)
 
     @classmethod
-    def from_token(cls, token, before=False):
+    def from_token(cls, token: Token, before: bool = False) -> 'EOS':
         col_offset = token.col_offset if before else token.end_col_offset
-        return EOS(token.lineno, col_offset)
+        return cls(token.lineno, col_offset)
 
 
 class END(Token):
     """Token representing END token used to signify block ending.
 
     Virtual END tokens have '' as their value, with "real" END tokens the
     value is 'END'.
     """
     __slots__ = []
 
-    def __init__(self, lineno=-1, col_offset=-1, virtual=False):
+    def __init__(self, lineno: int = -1, col_offset: int = -1, virtual: bool = False):
         value = 'END' if not virtual else ''
-        Token.__init__(self, Token.END, value, lineno, col_offset)
+        super().__init__(Token.END, value, lineno, col_offset)
 
     @classmethod
-    def from_token(cls, token, virtual=False):
-        return END(token.lineno, token.end_col_offset, virtual)
+    def from_token(cls, token: Token, virtual: bool = False) -> 'END':
+        return cls(token.lineno, token.end_col_offset, virtual)
```

## Comparing `robotframework-6.1a1/src/robot/parsing/lexer/__init__.py` & `robotframework-6.1b1/src/robot/parsing/lexer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from .lexer import get_tokens, get_resource_tokens, get_init_tokens
-from .tokens import Token
+from .tokens import StatementTokens, Token
```

## Comparing `robotframework-6.1a1/src/robot/parsing/lexer/tokenizer.py` & `robotframework-6.1b1/src/robot/parsing/lexer/tokenizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re
+from collections.abc import Iterator
 
 from .tokens import Token
 
 
 class Tokenizer:
     _space_splitter = re.compile(r'(\s{2,}|\t)', re.UNICODE)
     _pipe_splitter = re.compile(r'((?:\A|\s+)\|(?:\s+|\Z))', re.UNICODE)
 
-    def tokenize(self, data, data_only=False):
-        current = []
+    def tokenize(self, data: str, data_only: bool = False) -> 'Iterator[list[Token]]':
+        current: 'list[Token]' = []
         for lineno, line in enumerate(data.splitlines(not data_only), start=1):
             tokens = self._tokenize_line(line, lineno, not data_only)
             tokens, starts_new = self._cleanup_tokens(tokens, data_only)
             if starts_new:
                 if current:
                     yield current
                 current = tokens
             else:
                 current.extend(tokens)
         yield current
 
-    def _tokenize_line(self, line, lineno, include_separators=True):
+    def _tokenize_line(self, line: str, lineno: int, include_separators: bool):
         # Performance optimized code.
-        tokens = []
+        tokens: 'list[Token]' = []
         append = tokens.append
         offset = 0
         if line[:1] == '|' and line[:2].strip() == '|':
             splitter = self._split_from_pipes
         else:
             splitter = self._split_from_spaces
         for value, is_data in splitter(line.rstrip()):
@@ -51,87 +52,87 @@
                 append(Token(Token.SEPARATOR, value, lineno, offset))
             offset += len(value)
         if include_separators:
             trailing_whitespace = line[len(line.rstrip()):]
             append(Token(Token.EOL, trailing_whitespace, lineno, offset))
         return tokens
 
-    def _split_from_spaces(self, line):
+    def _split_from_spaces(self, line: str) -> 'Iterator[tuple[str, bool]]':
         is_data = True
         for value in self._space_splitter.split(line):
             yield value, is_data
             is_data = not is_data
 
-    def _split_from_pipes(self, line):
+    def _split_from_pipes(self, line) -> 'Iterator[tuple[str, bool]]':
         splitter = self._pipe_splitter
         _, separator, rest = splitter.split(line, 1)
         yield separator, False
         while splitter.search(rest):
             token, separator, rest = splitter.split(rest, 1)
             yield token, True
             yield separator, False
         yield rest, True
 
-    def _cleanup_tokens(self, tokens, data_only):
-        has_data, continues = self._handle_comments_and_continuation(tokens)
+    def _cleanup_tokens(self, tokens: 'list[Token]', data_only: bool):
+        has_data, has_comments, continues \
+                = self._handle_comments_and_continuation(tokens)
         self._remove_trailing_empty(tokens)
         if continues:
             self._remove_leading_empty(tokens)
             if not has_data:
                 self._ensure_data_after_continuation(tokens)
             starts_new = False
         else:
             starts_new = has_data
-        if data_only:
-            tokens = self._remove_non_data(tokens)
+        if data_only and (has_comments or continues):
+            tokens = [t for t in tokens if t.type is None]
         return tokens, starts_new
 
-    def _handle_comments_and_continuation(self, tokens):
+    def _handle_comments_and_continuation(self, tokens: 'list[Token]') \
+            -> 'tuple[bool, bool, bool]':
         has_data = False
-        continues = False
         commented = False
-        for token in tokens:
+        continues = False
+        for index, token in enumerate(tokens):
             if token.type is None:
                 # lstrip needed to strip possible leading space from first token.
                 # Other leading/trailing spaces have been consumed as separators.
-                value = token.value.lstrip()
+                value = token.value if index else token.value.lstrip()
                 if commented:
                     token.type = Token.COMMENT
                 elif value:
                     if value[0] == '#':
                         token.type = Token.COMMENT
                         commented = True
                     elif not has_data:
                         if value == '...' and not continues:
                             token.type = Token.CONTINUATION
                             continues = True
                         else:
                             has_data = True
-        return has_data, continues
+        return has_data, commented, continues
 
-    def _remove_trailing_empty(self, tokens):
+    def _remove_trailing_empty(self, tokens: 'list[Token]'):
         for token in reversed(tokens):
             if not token.value and token.type != Token.EOL:
                 tokens.remove(token)
             elif token.type is None:
                 break
 
-    def _remove_leading_empty(self, tokens):
+    def _remove_leading_empty(self, tokens: 'list[Token]'):
         data_or_continuation = (None, Token.CONTINUATION)
         for token in list(tokens):
             if not token.value:
                 tokens.remove(token)
             elif token.type in data_or_continuation:
                 break
 
-    def _ensure_data_after_continuation(self, tokens):
+    def _ensure_data_after_continuation(self, tokens: 'list[Token]'):
         cont = self._find_continuation(tokens)
         token = Token(lineno=cont.lineno, col_offset=cont.end_col_offset)
         tokens.insert(tokens.index(cont) + 1, token)
 
-    def _find_continuation(self, tokens):
+    def _find_continuation(self, tokens: 'list[Token]') -> Token:
         for token in tokens:
             if token.type == Token.CONTINUATION:
                 return token
-
-    def _remove_non_data(self, tokens):
-        return [t for t in tokens if t.type is None]
+        raise ValueError('Continuation not found.')
```

## Comparing `robotframework-6.1a1/src/robot/libraries/XML.py` & `robotframework-6.1b1/src/robot/libraries/XML.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,28 +452,27 @@
     wildcards.
 
     Support for brackets like ``[abc]`` and ``[!a-z]`` is new in
     Robot Framework 3.1
     """
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
     ROBOT_LIBRARY_VERSION = get_version()
-    _xml_declaration = re.compile('^<\?xml .*\?>')
 
     def __init__(self, use_lxml=False):
         """Import library with optionally lxml mode enabled.
 
-        By default this library uses Python's standard
+        This library uses Python's standard
         [http://docs.python.org/library/xml.etree.elementtree.html|ElementTree]
-        module for parsing XML. If ``use_lxml`` argument is given a true value
-        (see `Boolean arguments`), the library will use [http://lxml.de|lxml]
-        module instead. See `Using lxml` section for benefits provided by lxml.
+        module for parsing XML by default. If ``use_lxml`` argument is given
+        a true value (see `Boolean arguments`), the [http://lxml.de|lxml] module
+        is used instead. See the `Using lxml` section for benefits provided by lxml.
 
         Using lxml requires that the lxml module is installed on the system.
         If lxml mode is enabled but the module is not installed, this library
-        will emit a warning and revert back to using the standard ElementTree.
+        emits a warning and reverts back to using the standard ElementTree.
         """
         use_lxml = is_truthy(use_lxml)
         if use_lxml and lxml_etree:
             self.etree = lxml_etree
             self.modern_etree = True
             self.lxml_etree = True
         else:
@@ -1298,23 +1297,23 @@
     def element_to_string(self, source, xpath='.', encoding=None):
         """Returns the string representation of the specified element.
 
         The element to convert to a string is specified using ``source`` and
         ``xpath``. They have exactly the same semantics as with `Get Element`
         keyword.
 
-        By default the string is returned as Unicode. If ``encoding`` argument
+        The string is returned as Unicode by default. If ``encoding`` argument
         is given any value, the string is returned as bytes in the specified
         encoding. The resulting string never contains the XML declaration.
 
         See also `Log Element` and `Save XML`.
         """
         source = self.get_element(source, xpath)
         string = self.etree.tostring(source, encoding='UTF-8').decode('UTF-8')
-        string = self._xml_declaration.sub('', string).strip()
+        string = re.sub(r'^<\?xml .*\?>', '', string).strip()
         if encoding:
             string = string.encode(encoding)
         return string
 
     def log_element(self, source, level='INFO', xpath='.'):
         """Logs the string representation of the specified element.
```

## Comparing `robotframework-6.1a1/src/robot/libraries/Screenshot.py` & `robotframework-6.1b1/src/robot/libraries/Screenshot.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Easter.py` & `robotframework-6.1b1/src/robot/libraries/Easter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/dialogs_py.py` & `robotframework-6.1b1/src/robot/libraries/dialogs_py.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/String.py` & `robotframework-6.1b1/src/robot/libraries/String.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Telnet.py` & `robotframework-6.1b1/src/robot/libraries/Telnet.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/DateTime.py` & `robotframework-6.1b1/src/robot/libraries/DateTime.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Remote.py` & `robotframework-6.1b1/src/robot/libraries/Remote.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/OperatingSystem.py` & `robotframework-6.1b1/src/robot/libraries/OperatingSystem.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Collections.py` & `robotframework-6.1b1/src/robot/libraries/Collections.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/__init__.py` & `robotframework-6.1b1/src/robot/libraries/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Reserved.py` & `robotframework-6.1b1/src/robot/libraries/Reserved.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Dialogs.py` & `robotframework-6.1b1/src/robot/libraries/Dialogs.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/BuiltIn.py` & `robotframework-6.1b1/src/robot/libraries/BuiltIn.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/libraries/Process.py` & `robotframework-6.1b1/src/robot/libraries/Process.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import os
 import signal as signal_module
 import subprocess
 import time
 from tempfile import TemporaryFile
 
-from robot.utils import (abspath, cmdline2list, ConnectionCache, console_decode,
-                         console_encode, is_list_like, is_pathlike, is_string,
-                         is_truthy, NormalizedDict, secs_to_timestr, system_decode,
-                         system_encode, timestr_to_secs, WINDOWS)
-from robot.version import get_version
 from robot.api import logger
+from robot.utils import (cmdline2list, ConnectionCache, console_decode, console_encode,
+                         is_list_like, is_pathlike, is_string, is_truthy,
+                         NormalizedDict, secs_to_timestr, system_decode, system_encode,
+                         timestr_to_secs, WINDOWS)
+from robot.version import get_version
 
 
 class Process:
     """Robot Framework library for running processes.
 
     This library utilizes Python's
     [http://docs.python.org/library/subprocess.html|subprocess]
@@ -409,16 +409,16 @@
         self._results[process] = ExecutionResult(process, **conf.result_config)
         self._processes.register(process, alias=conf.alias)
         return self._processes.current
 
     def _log_start(self, command, config):
         if is_list_like(command):
             command = self.join_command_line(command)
-        logger.info('Starting process:\n%s' % system_decode(command))
-        logger.debug('Process configuration:\n%s' % config)
+        logger.info(f'Starting process:\n{system_decode(command)}')
+        logger.debug(f'Process configuration:\n{config}')
 
     def is_process_running(self, handle=None):
         """Checks is the process running or not.
 
         If ``handle`` is not given, uses the current `active process`.
 
         Returns ``True`` if the process is still running and ``False`` otherwise.
@@ -497,16 +497,15 @@
         in Robot Framework 3.2.
         """
         process = self._processes[handle]
         logger.info('Waiting for process to complete.')
         timeout = self._get_timeout(timeout)
         if timeout > 0:
             if not self._process_is_stopped(process, timeout):
-                logger.info('Process did not complete in %s.'
-                            % secs_to_timestr(timeout))
+                logger.info(f'Process did not complete in {secs_to_timestr(timeout)}.')
                 return self._manage_process_timeout(handle, on_timeout.lower())
         return self._wait(process)
 
     def _get_timeout(self, timeout):
         if (is_string(timeout) and timeout.upper() == 'NONE') or not timeout:
             return -1
         return timestr_to_secs(timeout)
@@ -636,15 +635,15 @@
         To send the signal to the whole process group, ``group`` argument can
         be set to any true value (see `Boolean arguments`).
         """
         if os.sep == '\\':
             raise RuntimeError('This keyword does not work on Windows.')
         process = self._processes[handle]
         signum = self._get_signal_number(signal)
-        logger.info('Sending signal %s (%d).' % (signal, signum))
+        logger.info(f'Sending signal {signal} ({signum}).')
         if is_truthy(group) and hasattr(os, 'killpg'):
             os.killpg(process.pid, signum)
         elif hasattr(process, 'send_signal'):
             process.send_signal(signum)
         else:
             raise RuntimeError('Sending signals is not supported '
                                'by this Python version.')
@@ -656,15 +655,15 @@
             return self._convert_signal_name_to_number(int_or_name)
 
     def _convert_signal_name_to_number(self, name):
         try:
             return getattr(signal_module,
                            name if name.startswith('SIG') else 'SIG' + name)
         except AttributeError:
-            raise RuntimeError("Unsupported signal '%s'." % name)
+            raise RuntimeError(f"Unsupported signal '{name}'.")
 
     def get_process_id(self, handle=None):
         """Returns the process ID (pid) of the process as an integer.
 
         If ``handle`` is not given, uses the current `active process`.
 
         Starting from Robot Framework 5.0, it is also possible to directly access
@@ -765,42 +764,44 @@
             time.sleep(min(0.1, timeout))
         return stopped()
 
     def split_command_line(self, args, escaping=False):
         """Splits command line string into a list of arguments.
 
         String is split from spaces, but argument surrounded in quotes may
-        contain spaces in them. If ``escaping`` is given a true value, then
-        backslash is treated as an escape character. It can escape unquoted
-        spaces, quotes inside quotes, and so on, but it also requires using
-        double backslashes when using Windows paths.
+        contain spaces in them.
+
+        If ``escaping`` is given a true value, then backslash is treated as
+        an escape character. It can escape unquoted spaces, quotes inside
+        quotes, and so on, but it also requires using doubling backslashes
+        in Windows paths and elsewhere.
 
         Examples:
         | @{cmd} = | Split Command Line | --option "value with spaces" |
         | Should Be True | $cmd == ['--option', 'value with spaces'] |
         """
         return cmdline2list(args, escaping=escaping)
 
     def join_command_line(self, *args):
         """Joins arguments into one command line string.
 
         In resulting command line string arguments are delimited with a space,
         arguments containing spaces are surrounded with quotes, and possible
         quotes are escaped with a backslash.
 
-        If this keyword is given only one argument and that is a list like
+        If this keyword is given only one argument and that is a list-like
         object, then the values of that list are joined instead.
 
         Example:
         | ${cmd} = | Join Command Line | --option | value with spaces |
         | Should Be Equal | ${cmd} | --option "value with spaces" |
         """
         if len(args) == 1 and is_list_like(args[0]):
             args = args[0]
-        return subprocess.list2cmdline(args)
+        return subprocess.list2cmdline(str(a) for a in args)
 
 
 class ExecutionResult:
 
     def __init__(self, process, stdout, stderr, stdin=None, rc=None,
                  output_encoding=None):
         self._process = process
@@ -872,22 +873,22 @@
         if stdout:
             self._read_stdout()
         if stderr:
             self._read_stderr()
         return [stdin, stdout, stderr]
 
     def __str__(self):
-        return '<result object with rc %d>' % self.rc
+        return f'<result object with rc {self.rc}>'
 
 
 class ProcessConfiguration:
 
     def __init__(self, cwd=None, shell=False, stdout=None, stderr=None, stdin='PIPE',
                  output_encoding='CONSOLE', alias=None, env=None, **rest):
-        self.cwd = os.path.normpath(cwd) if cwd else abspath('.')
+        self.cwd = os.path.normpath(cwd) if cwd else os.path.abspath('.')
         self.shell = is_truthy(shell)
         self.alias = alias
         self.output_encoding = output_encoding
         self.stdout_stream = self._new_stream(stdout)
         self.stderr_stream = self._get_stderr(stderr, stdout, self.stdout_stream)
         self.stdin_stream = self._get_stdin(stdin)
         self.env = self._construct_env(env, rest)
@@ -939,19 +940,19 @@
         if env:
             return dict((system_encode(k), system_encode(env[k])) for k in env)
         if extra:
             return os.environ.copy()
         return None
 
     def _add_to_env(self, env, extra):
-        for key in extra:
-            if not key.startswith('env:'):
-                raise RuntimeError("Keyword argument '%s' is not supported by "
-                                   "this keyword." % key)
-            env[system_encode(key[4:])] = system_encode(extra[key])
+        for name in extra:
+            if not name.startswith('env:'):
+                raise RuntimeError(f"Keyword argument '{name}' is not supported by "
+                                   f"this keyword.")
+            env[system_encode(name[4:])] = system_encode(extra[name])
 
     def get_command(self, command, arguments):
         command = [system_encode(item) for item in [command] + arguments]
         if not self.shell:
             return command
         if arguments:
             return subprocess.list2cmdline(command)
@@ -982,28 +983,22 @@
     def result_config(self):
         return {'stdout': self.stdout_stream,
                 'stderr': self.stderr_stream,
                 'stdin': self.stdin_stream,
                 'output_encoding': self.output_encoding}
 
     def __str__(self):
-        return """\
-cwd:     %s
-shell:   %s
-stdout:  %s
-stderr:  %s
-stdin:   %s
-alias:   %s
-env:     %s""" % (self.cwd,
-                  self.shell,
-                  self._stream_name(self.stdout_stream),
-                  self._stream_name(self.stderr_stream),
-                  self._stream_name(self.stdin_stream),
-                  self.alias,
-                  self.env)
+        return f'''\
+cwd:     {self.cwd}
+shell:   {self.shell}
+stdout:  {self._stream_name(self.stdout_stream)}
+stderr:  {self._stream_name(self.stderr_stream)}
+stdin:   {self._stream_name(self.stdin_stream)}
+alias:   {self.alias}
+env:     {self.env}'''
 
     def _stream_name(self, stream):
         if hasattr(stream, 'name'):
             return stream.name
         return {subprocess.PIPE: 'PIPE',
                 subprocess.STDOUT: 'STDOUT',
                 None: 'None'}.get(stream, stream)
```

## Comparing `robotframework-6.1a1/src/robot/api/interfaces.py` & `robotframework-6.1b1/src/robot/api/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,58 +9,69 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""Optional base classes for libraries and listeners.
+"""Optional base classes for libraries and other extensions.
 
 Module contents:
 
 - :class:`DynamicLibrary` for libraries using the `dynamic library API`__.
 - :class:`HybridLibrary` for libraries using the `hybrid library API`__.
 - :class:`ListenerV2` for `listener interface version 2`__.
 - :class:`ListenerV3` for `listener interface version 3`__.
+- :class:`Parser` for `custom parsers`__. Also
+  :class:`~robot.running.builder.settings.TestDefaults` used in ``Parser``
+  type hints can be imported via this module if needed.
 - Type definitions used by the aforementioned classes.
 
 Main benefit of using these base classes is that editors can provide automatic
 completion, documentation and type information. Their usage is not required.
 Notice also that libraries typically use the static API and do not need any
 base class.
 
 .. note:: These classes are not exposed via the top level :mod:`robot.api`
           package and need to imported via :mod:`robot.api.interfaces`.
 
-.. note:: Using :class:`ListenerV2` and :class:`ListenerV3` requires Python 3.8
-          or newer.
+.. note:: Using this module requires having the typing_extensions__ module
+          installed when using Python 3.6 or 3.7.
 
-New in Robot Framework 6.1.
+This module is new in Robot Framework 6.1.
 
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#dynamic-library-api
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#hybrid-library-api
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#listener-version-2
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#listener-version-3
+__ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#parser-interface
+__ https://pypi.org/project/typing-extensions/
 """
 
 import sys
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 # Need to use version check and not try/except to support Mypy's stubgen.
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
-    TypedDict = dict
+    try:
+        from typing_extensions import TypedDict
+    except ImportError:
+        raise ImportError("Using the 'robot.api.interfaces' module requires having "
+                          "the 'typing_extensions' module installed with Python < 3.8.")
 if sys.version_info >= (3, 10):
     from types import UnionType
 else:
     UnionType = type
 
 from robot import result, running
 from robot.model import Message
+from robot.running import TestDefaults, TestSuite
 
 
 # Type aliases used by DynamicLibrary and HybridLibrary.
 Name = str
 PositArgs = List[Any]
 NamedArgs = Dict[str, Any]
 Documentation = str
@@ -503,15 +514,15 @@
         """Called when the whole execution ends.
 
         With library listeners called when the library goes out of scope.
         """
 
 
 class ListenerV3:
-    """Optional base class for listeners using the listener API v2."""
+    """Optional base class for listeners using the listener API v3."""
     ROBOT_LISTENER_API_VERSION = 3
 
     def start_suite(self, data: running.TestSuite, result: result.TestSuite):
         """Called when a suite starts."""
 
     def end_suite(self, data: running.TestSuite, result: result.TestSuite):
         """Called when a suite ends."""
@@ -556,7 +567,68 @@
         """Called after the debug file has been created."""
 
     def close(self):
         """Called when the whole execution ends.
 
         With library listeners called when the library goes out of scope.
         """
+
+
+class Parser(ABC):
+    """Optional base class for custom parsers.
+
+    Parsers do not need to explicitly extend this class and in simple cases
+    it is possible to implement them as modules. Regardless how a parser is
+    implemented, it must have :attr:`extension` attribute and :meth:`parse`
+    method. The :meth:`parse_init` method is optional and only needed if
+    a parser supports parsing suite initialization files.
+
+    The mandatory :attr:`extension` attribute specifies what file extension or
+    extensions a parser supports. It can be set either as a class or instance
+    attribute, and it can be either a string or a sequence of strings. The
+    attribute can also be named ``EXTENSION``, which typically works better
+    when a parser is implemented as a module.
+
+    Example::
+
+        from pathlib import Path
+        from robot.api import TestSuite
+        from robot.api.interfaces import Parser, TestDefaults
+
+
+        class ExampleParser(Parser):
+            extension = '.example'
+
+            def parse(self, source: Path, defaults: TestDefaults) -> TestSuite:
+                suite = TestSuite(TestSuite.name_from_source(source), source=source)
+                # parse the source file and add tests to the created suite
+                return suite
+
+    The support for custom parsers is new in Robot Framework 6.1.
+    """
+    extension: Union[str, Sequence[str]]
+
+    @abstractmethod
+    def parse(self, source: Path, defaults: TestDefaults) -> TestSuite:
+        """Mandatory method for parsing suite files.
+
+        :param source: Path to the file to parse.
+        :param defaults: Default values set for test in init files.
+
+        The ``defaults`` argument is optional. It is possible to implement
+        this method also so that it accepts only ``source``.
+        """
+        raise NotImplementedError
+
+    def parse_init(self, source: Path, defaults: TestDefaults) -> TestSuite:
+        """Optional method for parsing suite initialization files.
+
+        :param source: Path to the file to parse.
+        :param defaults: Default values to used with tests in child suites.
+
+        The ``defaults`` argument is optional. It is possible to implement
+        this method also so that it accepts only ``source``.
+
+        If this method is not implemented, possible initialization files cause
+        an error.
+        """
+        raise NotImplementedError
```

## Comparing `robotframework-6.1a1/src/robot/api/parsing.py` & `robotframework-6.1b1/src/robot/api/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 - :class:`~robot.parsing.model.statements.LibraryImport`
 - :class:`~robot.parsing.model.statements.ResourceImport`
 - :class:`~robot.parsing.model.statements.VariablesImport`
 - :class:`~robot.parsing.model.statements.Documentation`
 - :class:`~robot.parsing.model.statements.Metadata`
 - :class:`~robot.parsing.model.statements.ForceTags`
 - :class:`~robot.parsing.model.statements.DefaultTags`
+- :class:`~robot.parsing.model.statements.SuiteName`
 - :class:`~robot.parsing.model.statements.SuiteSetup`
 - :class:`~robot.parsing.model.statements.SuiteTeardown`
 - :class:`~robot.parsing.model.statements.TestSetup`
 - :class:`~robot.parsing.model.statements.TestTeardown`
 - :class:`~robot.parsing.model.statements.TestTemplate`
 - :class:`~robot.parsing.model.statements.TestTimeout`
 - :class:`~robot.parsing.model.statements.Variable`
@@ -507,14 +508,15 @@
 from robot.parsing.model.statements import (
     SectionHeader,
     LibraryImport,
     ResourceImport,
     VariablesImport,
     Documentation,
     Metadata,
+    SuiteName,
     SuiteSetup,
     SuiteTeardown,
     TestSetup,
     TestTeardown,
     TestTemplate,
     TestTimeout,
     ForceTags,
```

## Comparing `robotframework-6.1a1/src/robot/api/deco.py` & `robotframework-6.1b1/src/robot/api/deco.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/api/logger.py` & `robotframework-6.1b1/src/robot/api/logger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robot/api/__init__.py` & `robotframework-6.1b1/src/robot/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 * :mod:`.deco` module with decorators libraries can utilize.
 
 * :mod:`.exceptions` module containing exceptions that libraries can utilize for
   reporting failures and other events. These exceptions can be imported also directly
   via :mod:`robot.api` like ``from robot.api import SkipExecution``.
 
 * :mod:`.interfaces` module containing optional base classes that can be used
-  when creating libraries or listeners. New in Robot Framework 6.1.
+  when creating libraries and other extensions. New in Robot Framework 6.1.
 
 * :mod:`.parsing` module exposing the parsing APIs. This module is new in Robot
   Framework 4.0. Various parsing related functions and classes were exposed
   directly via :mod:`robot.api` already in Robot Framework 3.2, but they are
   effectively deprecated and will be removed in the future.
 
 * :class:`~robot.running.model.TestSuite` class for creating executable
```

## Comparing `robotframework-6.1a1/src/robot/api/exceptions.py` & `robotframework-6.1b1/src/robot/api/exceptions.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1a1/src/robotframework.egg-info/SOURCES.txt` & `robotframework-6.1b1/src/robotframework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,39 +27,44 @@
 src/robot/conf/gatherfailed.py
 src/robot/conf/languages.py
 src/robot/conf/settings.py
 src/robot/htmldata/__init__.py
 src/robot/htmldata/htmlfilewriter.py
 src/robot/htmldata/jsonwriter.py
 src/robot/htmldata/template.py
+src/robot/htmldata/common/__init__.py
 src/robot/htmldata/common/js_disabled.css
 src/robot/htmldata/common/storage.js
+src/robot/htmldata/lib/__init__.py
 src/robot/htmldata/lib/jquery.highlight.min.js
 src/robot/htmldata/lib/jquery.min.js
 src/robot/htmldata/lib/jquery.tablesorter.min.js
 src/robot/htmldata/lib/jquery.tmpl.min.js
 src/robot/htmldata/lib/jsxcompressor.min.js
+src/robot/htmldata/libdoc/__init__.py
 src/robot/htmldata/libdoc/doc_formatting.css
 src/robot/htmldata/libdoc/libdoc.css
 src/robot/htmldata/libdoc/libdoc.html
 src/robot/htmldata/libdoc/print.css
 src/robot/htmldata/libdoc/pygments.css
+src/robot/htmldata/rebot/__init__.py
 src/robot/htmldata/rebot/common.css
 src/robot/htmldata/rebot/doc_formatting.css
 src/robot/htmldata/rebot/fileloading.js
 src/robot/htmldata/rebot/log.css
 src/robot/htmldata/rebot/log.html
 src/robot/htmldata/rebot/log.js
 src/robot/htmldata/rebot/model.js
 src/robot/htmldata/rebot/print.css
 src/robot/htmldata/rebot/report.css
 src/robot/htmldata/rebot/report.html
 src/robot/htmldata/rebot/testdata.js
 src/robot/htmldata/rebot/util.js
 src/robot/htmldata/rebot/view.js
+src/robot/htmldata/testdoc/__init__.py
 src/robot/htmldata/testdoc/testdoc.css
 src/robot/htmldata/testdoc/testdoc.html
 src/robot/libdocpkg/__init__.py
 src/robot/libdocpkg/builder.py
 src/robot/libdocpkg/consoleviewer.py
 src/robot/libdocpkg/datatypes.py
 src/robot/libdocpkg/htmlutils.py
```

## Comparing `robotframework-6.1a1/src/robotframework.egg-info/PKG-INFO` & `robotframework-6.1b1/src/robotframework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: robotframework
-Version: 6.1a1
+Version: 6.1b1
 Summary: Generic automation framework for acceptance testing and robotic process automation (RPA)
 Home-page: https://robotframework.org
 Author: Pekka Klärck
 Author-email: peke@eliga.fi
 License: Apache License 2.0
 Download-URL: https://pypi.org/project/robotframework
 Project-URL: Source, https://github.com/robotframework/robotframework
 Project-URL: Issue Tracker, https://github.com/robotframework/robotframework/issues
 Project-URL: Documentation, https://robotframework.org/robotframework
-Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1a1.rst
+Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1b1.rst
 Project-URL: Slack, http://slack.robotframework.org
 Project-URL: Twitter, https://twitter.com/robotframework
 Description: Robot Framework
         ===============
         
         .. contents::
            :local:
```

