# Comparing `tmp/FantasyBaseballTrends-0.0.1.tar.gz` & `tmp/FantasyBaseballTrends-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FantasyBaseballTrends-0.0.1.tar", last modified: Tue Mar 28 18:48:44 2023, max compression
+gzip compressed data, was "FantasyBaseballTrends-0.1.2.tar", last modified: Fri May  5 19:11:15 2023, max compression
```

## Comparing `FantasyBaseballTrends-0.0.1.tar` & `FantasyBaseballTrends-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-03-28 18:48:44.646300 FantasyBaseballTrends-0.0.1/
--rw-r--r--   0 cargo      (501) staff       (20)      406 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/.bumpversion.cfg
-drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-03-28 18:48:44.641329 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/
--rw-r--r--   0 cargo      (501) staff       (20)     6372 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/FantasyBaseballTrends.py
--rw-r--r--   0 cargo      (501) staff       (20)       71 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/__init__.py
--rw-r--r--   0 cargo      (501) staff       (20)       63 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/__main__.py
--rw-r--r--   0 cargo      (501) staff       (20)       22 2023-03-28 17:42:32.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/_version.py
-drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-03-28 18:48:44.645565 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/
--rw-r--r--   0 cargo      (501) staff       (20)      184 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/AaronJudgeProj.csv
--rw-r--r--   0 cargo      (501) staff       (20)      576 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/JudgeCareerSplits.csv
--rw-r--r--   0 cargo      (501) staff       (20)     1476 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/JudgeLast10.csv
--rw-r--r--   0 cargo      (501) staff       (20)      814 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/JudgeLast5.csv
--rw-r--r--   0 cargo      (501) staff       (20)      290 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/JudgeLastGame.csv
--rw-r--r--   0 cargo      (501) staff       (20)      317 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/JudgeLhpCurrent.csv
--rw-r--r--   0 cargo      (501) staff       (20)      336 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/JudgeRhpCurrent.csv
--rw-r--r--   0 cargo      (501) staff       (20)     3899 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/test.py
-drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-03-28 18:48:44.642920 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/
--rw-r--r--   0 cargo      (501) staff       (20)     3007 2023-03-28 18:48:44.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/PKG-INFO
--rw-r--r--   0 cargo      (501) staff       (20)      817 2023-03-28 18:48:44.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/SOURCES.txt
--rw-r--r--   0 cargo      (501) staff       (20)        1 2023-03-28 18:48:44.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/dependency_links.txt
--rw-r--r--   0 cargo      (501) staff       (20)      192 2023-03-28 18:48:44.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/requires.txt
--rw-r--r--   0 cargo      (501) staff       (20)       22 2023-03-28 18:48:44.000000 FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/top_level.txt
--rw-r--r--   0 cargo      (501) staff       (20)    11357 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/LICENSE.md
--rw-r--r--   0 cargo      (501) staff       (20)      464 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/MANIFEST.in
--rw-r--r--   0 cargo      (501) staff       (20)     2388 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/Makefile
--rw-r--r--   0 cargo      (501) staff       (20)     3007 2023-03-28 18:48:44.645970 FantasyBaseballTrends-0.0.1/PKG-INFO
--rw-r--r--   0 cargo      (501) staff       (20)     2077 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/README.md
--rw-r--r--   0 cargo      (501) staff       (20)     2347 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/pyproject.toml
--rw-r--r--   0 cargo      (501) staff       (20)       38 2023-03-28 18:48:44.646396 FantasyBaseballTrends-0.0.1/setup.cfg
--rw-r--r--   0 cargo      (501) staff       (20)       39 2023-03-28 17:23:55.000000 FantasyBaseballTrends-0.0.1/setup.py
+drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-05-05 19:11:15.426474 FantasyBaseballTrends-0.1.2/
+-rw-r--r--   0 cargo      (501) staff       (20)      406 2023-05-04 22:26:12.000000 FantasyBaseballTrends-0.1.2/.bumpversion.cfg
+drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-05-05 19:11:15.420752 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/
+-rw-r--r--   0 cargo      (501) staff       (20)    13414 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/FantasyBaseballTrends.py
+-rw-r--r--   0 cargo      (501) staff       (20)       71 2023-05-05 06:35:46.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/__init__.py
+-rw-r--r--   0 cargo      (501) staff       (20)       63 2023-05-04 22:26:12.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/__main__.py
+-rw-r--r--   0 cargo      (501) staff       (20)       22 2023-05-05 18:54:11.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/_version.py
+drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-05-05 19:11:15.425465 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/
+-rw-r--r--   0 cargo      (501) staff       (20)      202 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/AaronJudgeCareer.csv
+-rw-r--r--   0 cargo      (501) staff       (20)     6609 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/AaronJudgePostseason.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      184 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/AaronJudgeSeason.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      579 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeCarrerSplits.csv
+-rw-r--r--   0 cargo      (501) staff       (20)     1500 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeLast10.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      304 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeLast10Avg.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      822 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeLast5.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      291 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeLastGame.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      317 2023-05-05 06:56:43.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeLhpCurrent.csv
+-rw-r--r--   0 cargo      (501) staff       (20)      336 2023-05-05 06:56:40.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/JudgeRhpCurrent.csv
+-rw-r--r--   0 cargo      (501) staff       (20)     5453 2023-05-05 18:14:51.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/test.py
+drwxr-xr-x   0 cargo      (501) staff       (20)        0 2023-05-05 19:11:15.422088 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/
+-rw-r--r--   0 cargo      (501) staff       (20)     3413 2023-05-05 19:11:14.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/PKG-INFO
+-rw-r--r--   0 cargo      (501) staff       (20)      968 2023-05-05 19:11:15.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/SOURCES.txt
+-rw-r--r--   0 cargo      (501) staff       (20)        1 2023-05-05 19:11:14.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/dependency_links.txt
+-rw-r--r--   0 cargo      (501) staff       (20)      192 2023-05-05 19:11:15.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/requires.txt
+-rw-r--r--   0 cargo      (501) staff       (20)       22 2023-05-05 19:11:15.000000 FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/top_level.txt
+-rw-r--r--   0 cargo      (501) staff       (20)    11357 2023-05-04 22:26:12.000000 FantasyBaseballTrends-0.1.2/LICENSE.md
+-rw-r--r--   0 cargo      (501) staff       (20)      464 2023-05-04 22:26:12.000000 FantasyBaseballTrends-0.1.2/MANIFEST.in
+-rw-r--r--   0 cargo      (501) staff       (20)     2388 2023-05-04 22:26:12.000000 FantasyBaseballTrends-0.1.2/Makefile
+-rw-r--r--   0 cargo      (501) staff       (20)     3413 2023-05-05 19:11:15.426062 FantasyBaseballTrends-0.1.2/PKG-INFO
+-rw-r--r--   0 cargo      (501) staff       (20)     2446 2023-05-05 18:14:42.000000 FantasyBaseballTrends-0.1.2/README.md
+-rw-r--r--   0 cargo      (501) staff       (20)     2347 2023-05-05 19:09:57.000000 FantasyBaseballTrends-0.1.2/pyproject.toml
+-rw-r--r--   0 cargo      (501) staff       (20)       38 2023-05-05 19:11:15.426602 FantasyBaseballTrends-0.1.2/setup.cfg
+-rw-r--r--   0 cargo      (501) staff       (20)       39 2023-05-04 22:26:12.000000 FantasyBaseballTrends-0.1.2/setup.py
```

### Comparing `FantasyBaseballTrends-0.0.1/FantasyBaseballTrends/tests/test.py` & `FantasyBaseballTrends-0.1.2/FantasyBaseballTrends/tests/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,17 +11,29 @@
         options = webdriver.ChromeOptions()
         # options.add_argument('headless')
         # options.page_load_strategy = 'eager'
         self.driver = webdriver.Chrome(options=options)
         self.driver.get("https://www.baseball-reference.com/")
 
     # test to see if the projected stats exist and returns data Frame
-    def test_get2023Projected(self):
+    def test_get2023Season(self):
         self.assertEqual(
-            type(fbt.get2023Projected(self.driver, "Aaron Judge")),
+            type(fbt.get2023Season(self.driver, "Aaron Judge")),
+            pd.DataFrame,
+        )
+
+    def test_getCareer(self):
+        self.assertEqual(
+            type(fbt.getCareer(self.driver, "Aaron Judge")),
+            pd.DataFrame,
+        )
+
+    def test_getPostseasonStats(self):
+        self.assertEqual(
+            type(fbt.getPostseasonStats(self.driver, "Aaron Judge")),
             pd.DataFrame,
         )
 
     # test to see if last game stats exist
     def test_getLastGame(self):
         self.assertEqual(
             type(fbt.getLastGame(self.driver, "Aaron Judge")), pd.DataFrame
@@ -47,30 +59,50 @@
 
     # test to see if carreer splits log exists
     def test_getCareerSplits(self):
         self.assertEqual(
             type(fbt.getCareerSplits(self.driver, "Aaron Judge")), pd.DataFrame
         )
 
-    def test_intget2023Projected(self):
+    def test_intget2023Season(self):
         testFrame = pd.read_csv(
-            'FantasyBaseballTrends/tests/AaronJudgeProj.csv', index_col=0
+            'FantasyBaseballTrends/tests/AaronJudgeSeason.csv', index_col=0
         )
         assert_frame_equal(
-            fbt.get2023Projected(self.driver, "Aaron Judge"), testFrame
+            fbt.get2023Season(self.driver, "Aaron Judge"),
+            testFrame,
+            check_dtype=False,
         )
 
     def test_intgetLastGame(self):
         testFrame = pd.read_csv(
             'FantasyBaseballTrends/tests/JudgeLastGame.csv',
             index_col=0,
             dtype=str,
         )
+        testFrame = testFrame.astype(str)
+        actualFrame = fbt.getLastGame(self.driver, "Aaron Judge")
+        actualFrame = actualFrame.astype(str)
+        assert_frame_equal(actualFrame, testFrame, check_dtype=False)
+
+    def test_intgetPostseason(self):
+        testFrame = pd.read_csv(
+            'FantasyBaseballTrends/tests/AaronJudgePostseason.csv', index_col=0
+        )
+        testFrame = testFrame.astype(str)
+        actualFrame = fbt.getPostseasonStats(self.driver, "Aaron Judge")
+        actualFrame = actualFrame.astype(str)
+        assert_frame_equal(actualFrame, testFrame, check_dtype=False)
+
+    def test_intgetCareer(self):
+        testFrame = pd.read_csv(
+            'FantasyBaseballTrends/tests/AaronJudgeCareer.csv', index_col=0
+        )
         assert_frame_equal(
-            fbt.getLastGame(self.driver, "Aaron Judge"),
+            fbt.getCareer(self.driver, "Aaron Judge"),
             testFrame,
             check_dtype=False,
         )
 
     def test_intgetRhpCurrent(self):
         testFrame = pd.read_csv(
             'FantasyBaseballTrends/tests/JudgeRhpCurrent.csv', index_col=0
@@ -85,44 +117,56 @@
         )
         assert_frame_equal(
             fbt.getVsLhpCurrent(self.driver, "Aaron Judge"), testFrame
         )
 
     def test_intgetCarrerSplits(self):
         testFrame = pd.read_csv(
-            'FantasyBaseballTrends/tests/JudgeCareerSplits.csv', index_col=0
+            'FantasyBaseballTrends/tests/JudgeCarrerSplits.csv', index_col=0
         )
         assert_frame_equal(
             fbt.getCareerSplits(self.driver, "Aaron Judge"), testFrame
         )
 
     def test_intgetLastxGames1(self):
         testFrame = pd.read_csv(
             'FantasyBaseballTrends/tests/JudgeLast5.csv',
             index_col=0,
             dtype=str,
         )
+        testFrame = testFrame.astype(str)
+        actualFrame = fbt.getLastxGames(self.driver, "Aaron Judge", 5)
+        actualFrame = actualFrame.astype(str)
         assert_frame_equal(
-            fbt.getLastxGames(self.driver, "Aaron Judge", 5),
+            actualFrame,
             testFrame,
             check_dtype=False,
         )
 
     def test_intgetLastxGames2(self):
         testFrame = pd.read_csv(
             'FantasyBaseballTrends/tests/JudgeLast10.csv',
             index_col=0,
             dtype=str,
         )
+        testFrame = testFrame.astype(str)
+        actualFrame = fbt.getLastxGames(self.driver, "Aaron Judge", 10)
+        actualFrame = actualFrame.astype(str)
         assert_frame_equal(
-            fbt.getLastxGames(self.driver, "Aaron Judge", 10),
+            actualFrame,
             testFrame,
             check_dtype=False,
         )
 
+    def test_intgetAvgOverLastxGames(self):
+        self.assertEqual(
+            type(fbt.getAvgOverLastxGames(self.driver, "Aaron Judge", 10)),
+            pd.DataFrame,
+        )
+
     # make a teardown
     def tearDown(self):
         self.driver.quit()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/PKG-INFO` & `FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: FantasyBaseballTrends
-Version: 0.0.1
+Version: 0.1.2
 Summary: Library that helps you search for baseball players stats and trends in order to help with fantasy lineup construction
 Author-email: Carlos Gonzalez-Romero <cmg2249@columbia.edu>
+License: UNKNOWN
 Project-URL: repository, https://github.com/Cargo1284/FantasyBaseballTrends
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,14 +22,18 @@
 
 # FantasyBaseballTrends
 
 [![Build Status](https://github.com/Cargo1284/FantasyBaseballTrends/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/Cargo1284/FantasyBaseballTrends/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/Cargo1284/FantasyBaseballTrends/branch/main/graph/badge.svg)](https://app.codecov.io/gh/Cargo1284/FantasyBaseballTrends)
 ![Crates.io](https://img.shields.io/crates/l/ap)
 ![GitHub issues](https://img.shields.io/github/issues/cargo1284/fantasybaseballtrends)
+[![PyPI](https://img.shields.io/pypi/v/FantasyBaseballTrends)](https://pypi.org/project/FantasyBaseballTrends/)
+[![Github Pages Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://cargo1284.github.io/FantasyBaseballTrends/)
+[![readthedocs](https://img.shields.io/readthedocs/fantasybaseballtrends)](https://fantasybaseballtrends.readthedocs.io/en/latest)
+
 
 
 ## Overview
 
 This library scrapes specific hitter stats from BaseballReference.
 The purpose of this library is to provide fantasy owners a chance to see how the players in their lineup have been performing over a number of games and how they perform against a certain pitcher. This will help facilitate their daily lineup constuction and to see which players on the wire are having a hot streak as well as players that have been trending downwards. 
 
@@ -65,7 +71,9 @@
 ```
 ### Stats over number of games
 This funciton will return a hitter's stats over a user specified number of games. 
 ```
 getLastxGames(browser, player, gamesNum)
 ```
 
+
+
```

### Comparing `FantasyBaseballTrends-0.0.1/FantasyBaseballTrends.egg-info/SOURCES.txt` & `FantasyBaseballTrends-0.1.2/FantasyBaseballTrends.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 FantasyBaseballTrends/__main__.py
 FantasyBaseballTrends/_version.py
 FantasyBaseballTrends.egg-info/PKG-INFO
 FantasyBaseballTrends.egg-info/SOURCES.txt
 FantasyBaseballTrends.egg-info/dependency_links.txt
 FantasyBaseballTrends.egg-info/requires.txt
 FantasyBaseballTrends.egg-info/top_level.txt
-FantasyBaseballTrends/tests/AaronJudgeProj.csv
-FantasyBaseballTrends/tests/JudgeCareerSplits.csv
+FantasyBaseballTrends/tests/AaronJudgeCareer.csv
+FantasyBaseballTrends/tests/AaronJudgePostseason.csv
+FantasyBaseballTrends/tests/AaronJudgeSeason.csv
+FantasyBaseballTrends/tests/JudgeCarrerSplits.csv
 FantasyBaseballTrends/tests/JudgeLast10.csv
+FantasyBaseballTrends/tests/JudgeLast10Avg.csv
 FantasyBaseballTrends/tests/JudgeLast5.csv
 FantasyBaseballTrends/tests/JudgeLastGame.csv
 FantasyBaseballTrends/tests/JudgeLhpCurrent.csv
 FantasyBaseballTrends/tests/JudgeRhpCurrent.csv
 FantasyBaseballTrends/tests/test.py
```

### Comparing `FantasyBaseballTrends-0.0.1/LICENSE.md` & `FantasyBaseballTrends-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FantasyBaseballTrends-0.0.1/Makefile` & `FantasyBaseballTrends-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `FantasyBaseballTrends-0.0.1/PKG-INFO` & `FantasyBaseballTrends-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: FantasyBaseballTrends
-Version: 0.0.1
+Version: 0.1.2
 Summary: Library that helps you search for baseball players stats and trends in order to help with fantasy lineup construction
 Author-email: Carlos Gonzalez-Romero <cmg2249@columbia.edu>
+License: UNKNOWN
 Project-URL: repository, https://github.com/Cargo1284/FantasyBaseballTrends
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,14 +22,18 @@
 
 # FantasyBaseballTrends
 
 [![Build Status](https://github.com/Cargo1284/FantasyBaseballTrends/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/Cargo1284/FantasyBaseballTrends/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/Cargo1284/FantasyBaseballTrends/branch/main/graph/badge.svg)](https://app.codecov.io/gh/Cargo1284/FantasyBaseballTrends)
 ![Crates.io](https://img.shields.io/crates/l/ap)
 ![GitHub issues](https://img.shields.io/github/issues/cargo1284/fantasybaseballtrends)
+[![PyPI](https://img.shields.io/pypi/v/FantasyBaseballTrends)](https://pypi.org/project/FantasyBaseballTrends/)
+[![Github Pages Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://cargo1284.github.io/FantasyBaseballTrends/)
+[![readthedocs](https://img.shields.io/readthedocs/fantasybaseballtrends)](https://fantasybaseballtrends.readthedocs.io/en/latest)
+
 
 
 ## Overview
 
 This library scrapes specific hitter stats from BaseballReference.
 The purpose of this library is to provide fantasy owners a chance to see how the players in their lineup have been performing over a number of games and how they perform against a certain pitcher. This will help facilitate their daily lineup constuction and to see which players on the wire are having a hot streak as well as players that have been trending downwards. 
 
@@ -65,7 +71,9 @@
 ```
 ### Stats over number of games
 This funciton will return a hitter's stats over a user specified number of games. 
 ```
 getLastxGames(browser, player, gamesNum)
 ```
 
+
+
```

### Comparing `FantasyBaseballTrends-0.0.1/README.md` & `FantasyBaseballTrends-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # FantasyBaseballTrends
 
 [![Build Status](https://github.com/Cargo1284/FantasyBaseballTrends/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/Cargo1284/FantasyBaseballTrends/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/Cargo1284/FantasyBaseballTrends/branch/main/graph/badge.svg)](https://app.codecov.io/gh/Cargo1284/FantasyBaseballTrends)
 ![Crates.io](https://img.shields.io/crates/l/ap)
 ![GitHub issues](https://img.shields.io/github/issues/cargo1284/fantasybaseballtrends)
+[![PyPI](https://img.shields.io/pypi/v/FantasyBaseballTrends)](https://pypi.org/project/FantasyBaseballTrends/)
+[![Github Pages Docs](https://img.shields.io/badge/docs-gh--pages-blue)](https://cargo1284.github.io/FantasyBaseballTrends/)
+[![readthedocs](https://img.shields.io/readthedocs/fantasybaseballtrends)](https://fantasybaseballtrends.readthedocs.io/en/latest)
+
 
 
 ## Overview
 
 This library scrapes specific hitter stats from BaseballReference.
 The purpose of this library is to provide fantasy owners a chance to see how the players in their lineup have been performing over a number of games and how they perform against a certain pitcher. This will help facilitate their daily lineup constuction and to see which players on the wire are having a hot streak as well as players that have been trending downwards.
```

### Comparing `FantasyBaseballTrends-0.0.1/pyproject.toml` & `FantasyBaseballTrends-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "FantasyBaseballTrends"
 authors = [{name = "Carlos Gonzalez-Romero", email = "cmg2249@columbia.edu"}]
 description="Library that helps you search for baseball players stats and trends in order to help with fantasy lineup construction"
 readme = "README.md"
-version = "0.0.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = [ 
     "selenium", 
     "pandas",
     "beautifulsoup4",
     "lxml"
```

