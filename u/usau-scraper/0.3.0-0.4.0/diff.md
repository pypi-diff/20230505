# Comparing `tmp/usau-scraper-0.3.0.tar.gz` & `tmp/usau-scraper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usau-scraper-0.3.0.tar", last modified: Tue Apr 25 16:33:50 2023, max compression
+gzip compressed data, was "usau-scraper-0.4.0.tar", last modified: Thu May  4 23:57:46 2023, max compression
```

## Comparing `usau-scraper-0.3.0.tar` & `usau-scraper-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,51 @@
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.166925 usau-scraper-0.3.0/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      301 2023-04-25 16:26:11.000000 usau-scraper-0.3.0/.bumpversion.cfg
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      551 2023-04-24 21:18:45.000000 usau-scraper-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    11357 2023-02-07 19:30:12.000000 usau-scraper-0.3.0/LICENSE
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      536 2023-04-04 20:12:02.000000 usau-scraper-0.3.0/MANIFEST.in
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2630 2023-04-25 15:43:37.000000 usau-scraper-0.3.0/Makefile
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    19732 2023-04-25 16:33:50.166563 usau-scraper-0.3.0/PKG-INFO
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     5805 2023-04-25 16:22:47.000000 usau-scraper-0.3.0/README.md
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.156752 usau-scraper-0.3.0/docs/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      638 2023-04-03 14:59:19.000000 usau-scraper-0.3.0/docs/Makefile
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      799 2023-04-03 14:59:19.000000 usau-scraper-0.3.0/docs/make.bat
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.158780 usau-scraper-0.3.0/docs/source/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2029 2023-04-04 18:50:42.000000 usau-scraper-0.3.0/docs/source/conf.py
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1722 2023-04-25 16:04:54.000000 usau-scraper-0.3.0/docs/source/index.rst
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      191 2023-04-25 16:06:05.000000 usau-scraper-0.3.0/docs/source/modules.rst
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.159939 usau-scraper-0.3.0/examples/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    33908 2023-04-05 15:20:17.000000 usau-scraper-0.3.0/examples/usau_scraper_example.ipynb
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2329 2023-04-25 16:26:11.000000 usau-scraper-0.3.0/pyproject.toml
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)       38 2023-04-25 16:33:50.167009 usau-scraper-0.3.0/setup.cfg
--rw-rw-r--   0 theodoremcnulty   (501) staff       (20)       39 2023-02-27 18:37:36.000000 usau-scraper-0.3.0/setup.py
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.162509 usau-scraper-0.3.0/usau_scraper/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      249 2023-04-25 16:26:11.000000 usau-scraper-0.3.0/usau_scraper/__init__.py
--rw-rw-r--   0 theodoremcnulty   (501) staff       (20)      118 2023-03-08 19:58:10.000000 usau-scraper-0.3.0/usau_scraper/__main__.py
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    13589 2023-04-25 16:22:26.000000 usau-scraper-0.3.0/usau_scraper/teamScraper.py
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.164765 usau-scraper-0.3.0/usau_scraper/tests/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     5630 2023-04-25 16:17:46.000000 usau-scraper-0.3.0/usau_scraper/tests/test_all.py
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1233 2023-03-08 16:58:23.000000 usau-scraper-0.3.0/usau_scraper/tournamentScraper.py
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.165996 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    15801 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/PKG-INFO
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      383 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/requires.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)       55 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.164519 usau-scraper-0.3.0/usau_scraper.egg-info/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    19732 2023-04-25 16:33:49.000000 usau-scraper-0.3.0/usau_scraper.egg-info/PKG-INFO
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      791 2023-04-25 16:33:50.000000 usau-scraper-0.3.0/usau_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-04-25 16:33:49.000000 usau-scraper-0.3.0/usau_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-04-25 16:33:49.000000 usau-scraper-0.3.0/usau_scraper.egg-info/requires.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)       13 2023-04-25 16:33:50.000000 usau-scraper-0.3.0/usau_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.256180 usau-scraper-0.4.0/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      301 2023-05-04 23:53:43.000000 usau-scraper-0.4.0/.bumpversion.cfg
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      667 2023-05-04 23:31:22.000000 usau-scraper-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    11357 2023-02-07 19:30:12.000000 usau-scraper-0.4.0/LICENSE
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      566 2023-05-04 23:38:29.000000 usau-scraper-0.4.0/MANIFEST.in
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2630 2023-05-04 23:57:30.000000 usau-scraper-0.4.0/Makefile
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    17920 2023-05-04 23:57:46.255902 usau-scraper-0.4.0/PKG-INFO
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     3993 2023-05-04 23:53:28.000000 usau-scraper-0.4.0/README.md
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.225121 usau-scraper-0.4.0/docs/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      638 2023-04-03 14:59:19.000000 usau-scraper-0.4.0/docs/Makefile
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.225854 usau-scraper-0.4.0/docs/assets/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)   288160 2023-05-04 23:38:29.000000 usau-scraper-0.4.0/docs/assets/project-logo.png
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.220218 usau-scraper-0.4.0/docs/build/
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.220481 usau-scraper-0.4.0/docs/build/html/
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.228750 usau-scraper-0.4.0/docs/build/html/_images/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)   288160 2023-04-28 15:14:36.000000 usau-scraper-0.4.0/docs/build/html/_images/project-logo.png
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.232598 usau-scraper-0.4.0/docs/build/html/_static/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      286 2021-05-11 23:58:54.000000 usau-scraper-0.4.0/docs/build/html/_static/file.png
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       90 2021-05-11 23:58:54.000000 usau-scraper-0.4.0/docs/build/html/_static/minus.png
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       90 2021-05-11 23:58:54.000000 usau-scraper-0.4.0/docs/build/html/_static/plus.png
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      799 2023-04-03 14:59:19.000000 usau-scraper-0.4.0/docs/make.bat
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.235021 usau-scraper-0.4.0/docs/source/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2029 2023-04-04 18:50:42.000000 usau-scraper-0.4.0/docs/source/conf.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1791 2023-05-04 23:38:29.000000 usau-scraper-0.4.0/docs/source/developer.rst
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2282 2023-05-04 23:53:28.000000 usau-scraper-0.4.0/docs/source/index.rst
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      418 2023-05-04 23:38:29.000000 usau-scraper-0.4.0/docs/source/modules.rst
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.235583 usau-scraper-0.4.0/examples/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    33934 2023-05-04 23:31:22.000000 usau-scraper-0.4.0/examples/usau_scraper_example.ipynb
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2329 2023-05-04 23:53:43.000000 usau-scraper-0.4.0/pyproject.toml
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       38 2023-05-04 23:57:46.256262 usau-scraper-0.4.0/setup.cfg
+-rw-rw-r--   0 theodoremcnulty   (501) staff       (20)       39 2023-02-27 18:37:36.000000 usau-scraper-0.4.0/setup.py
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.237646 usau-scraper-0.4.0/usau_scraper/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      698 2023-05-04 23:53:43.000000 usau-scraper-0.4.0/usau_scraper/__init__.py
+-rw-rw-r--   0 theodoremcnulty   (501) staff       (20)      118 2023-05-04 23:18:18.000000 usau-scraper-0.4.0/usau_scraper/__main__.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2945 2023-05-04 23:32:08.000000 usau-scraper-0.4.0/usau_scraper/rankingScraper.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    13589 2023-04-25 16:22:26.000000 usau-scraper-0.4.0/usau_scraper/teamScraper.py
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.254029 usau-scraper-0.4.0/usau_scraper/tests/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     8523 2023-05-04 23:40:19.000000 usau-scraper-0.4.0/usau_scraper/tests/test_all.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    13842 2023-05-04 23:38:29.000000 usau-scraper-0.4.0/usau_scraper/tournamentScraper.py
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.255480 usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    15801 2023-03-02 18:55:12.000000 usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      383 2023-03-02 18:55:12.000000 usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-03-02 18:55:12.000000 usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-03-02 18:55:12.000000 usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/requires.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       55 2023-03-02 18:55:12.000000 usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-05-04 23:57:46.238861 usau-scraper-0.4.0/usau_scraper.egg-info/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    17920 2023-05-04 23:57:45.000000 usau-scraper-0.4.0/usau_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1018 2023-05-04 23:57:46.000000 usau-scraper-0.4.0/usau_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-05-04 23:57:45.000000 usau-scraper-0.4.0/usau_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-05-04 23:57:46.000000 usau-scraper-0.4.0/usau_scraper.egg-info/requires.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       13 2023-05-04 23:57:46.000000 usau-scraper-0.4.0/usau_scraper.egg-info/top_level.txt
```

### Comparing `usau-scraper-0.3.0/LICENSE` & `usau-scraper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/MANIFEST.in` & `usau-scraper-0.4.0/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 include Makefile
 
 recursive-include docs *.bat
 recursive-include docs *.rst
 recursive-include docs *.py
 recursive-include examples *.ipynb
 recursive-include docs Makefile
+recursive-include docs *.png
+
 
 prune .github
 exclude .gitignore
 exclude .gitattributes
 
 # Patterns to exclude from any directory
 global-exclude *~
```

### Comparing `usau-scraper-0.3.0/Makefile` & `usau-scraper-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/PKG-INFO` & `usau-scraper-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usau-scraper
-Version: 0.3.0
+Version: 0.4.0
 Summary: The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the USAU website.
 Author-email: Erin McNulty <eem2188@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,15 +217,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# USAU Scraper
+<p align="center">
+<img width="500" alt="USAU logo surrounded by data icons" src="https://user-images.githubusercontent.com/16248113/235183543-063d7200-5dcb-491d-bdbe-2eeaea6b5eee.png">
+</p>
 
 The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the [USAU website](https://play.usaultimate.org/events/tournament/?ViewAll=false&IsLeagueType=false&IsClinic=false&FilterByCategory=AE).
 
 ![Apache Liscence](https://img.shields.io/github/license/erin2722/usau-scraper?color=f72d2d)
 
 [![PyPI](https://img.shields.io/pypi/v/usau-scraper?color=2d2df7)](https://pypi.org/project/usau-scraper/)
 
@@ -238,160 +240,65 @@
 
 ## Overview
 
 USAU (USA Ultimate) is the governing body of ultimate frisbee, and its website (which is notoriously hard to navigate) contains all of the information about high school, college, and club ultimate frisbee teams. Right now, there is no easy way to access this data. USAU scraper solves this problem by scraping the USAU website for data and therefore allowing other developers to easily use the data on the USAU site. This project will open the door to more data analytic projects concerning ultimate frisbee.
 
 ## Installation
 
-`pip install usau-scraper`
-
-## How to Use
-
-After installing the library, there are currently 3 functions available for use: getTeamInfo, getTeamSchedule, and getTeamRoster.
-
-Simply `import * from usau_scraper`, and then call any of the following functions:
-
-### getTeamInfo()
-
-`getTeamInfo()` returns all information about the first 20 teams matching the query
-
-**Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
-
-**Output:**
-
-```
-{
-    res: OK, NOTFOUND
-    teams: [
-        {
-            schoolName,
-            teamName,
-            competitionLevel,
-            genderDivision,
-            location,
-            coaches,
-            website,
-            facebook,
-            twitter,
-        },
-        ...
-    ]
-}
-```
-
-### getTeamSchedule
-
-`getTeamSchedule()` returns the season schedule and record of the first 20 teams matching the query
-
-**Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
-
-**Output:**
-
-```
-{
-    res: OK, NOTFOUND
-    teams: [
-        {
-            schoolName,
-            teamName,
-            competitionLevel,
-            genderDivision,
-            wins,
-            losses,
-            tournaments: {
-                name: {
-                    games: [
-                        {
-                            date,
-                            score,
-                            opponentCollege,
-                            opponentTeamPage
-                        },
-                        ...
-                    ]
-                },
-                ...
-            },
-        },
-        ...
-    ]
-}
-```
-
-### getTeamRoster
-
-`getTeamRoster()` returns the roster of the first 20 teams matching the query
-
-**Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
-
-**Output:**
-
-```
-{
-    res: OK, NOTFOUND
-    teams: [
-        {
-            schoolName,
-            teamName,
-            competitionLevel,
-            genderDivision,
-            roster: [
-                {
-                    no,
-                    name,
-                    pronouns,
-                    position,
-                    year,
-                    height,
-                },
-                ...
-            ]
-        },
-        ...
-    ]
-}
-```
+`pip install --upgrade usau-scraper`
 
 ## Example Usage
 
-After `pip install --upgrade usau-scraper` in your python env:
-
 ```python
-from usau_scraper import getTeamInfo, getTeamSchedule, getTeamRoster
+from usau_scraper import *
 
 # Get a team's basic information
 print(getTeamInfo(
-    schoolName = 'Columbia', 
-    teamName = 'Baewatch', 
-    genderDivision=2, 
-    state='NY', 
-    competitionLevel='College', 
-    competitionDivision=1, 
-    teamDesignation=1))
+    schoolName = 'Columbia',
+    teamName = 'Baewatch',
+    genderDivision='Women',
+    state='NY',
+    competitionLevel='College',
+    competitionDivision='Division 1',
+    teamDesignation='B'))
 
 # Get a team's schedule for the current season
 print(getTeamSchedule(schoolName='Columbia', teamName='Curbside'))
 
 # Get a team's roster for the current season
 print(getTeamRoster(schoolName='Columbia', teamName='Curbside'))
+
+# Get the pool play results for a tournament
+print(getTournamentPoolPlayResults("College", "Women", eventName="No Sleep Till Brooklyn", season=2023))
+
+# Get the bracket results for a tournament
+print(getTournamentBracketResults("College", "Women", eventName="Centex", season=2022))
+
+# Get the winner for a tournament
+print(getTournamentWinner("College", "Women", eventName="Stanford Invite", season=2023))
+
+# Get the top 20 women's college teams
+print(getCollegeRankings(genderDivision="Women"))
+
+# Get the top 20 women's club teams
+print(getClubRankings(genderDivision="Women"))
 ```
 
 Additional usage examples are [in this notebook](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb#scrollTo=20Fjgtxr35ES).
 
 ## Features (MVP)
 
 - [x] A function that, given a team name, returns basic information about them.
 - [x] A function that, given a team name, returns their schedule and record.
 - [x] A function that, given a team name, returns its roster.
-- [ ] A function that, given a tournament name, returns the results of the tournament.
+- [x] A function that, given a tournament name, returns the results of the tournament.
 
 ## Additional features
 
-- [ ] A function that, given a college division, returns the current standings of that division.
-- [ ] An additional plugin to [frisbee-rankings.com](http://www.frisbee-rankings.com/) to show current top 25 teams.
+- [x] A function that, given a college division, returns the current standings of that division.
 - [ ] An additional plugin to ultiworld to show recent articles given a team name or college division.
 - [ ] More features tbd!
 
 ## Possible Applications
 
 - A seeding helper that, given a list of team names, returns their records for the season and their record against top 25 teams.
```

### Comparing `usau-scraper-0.3.0/docs/Makefile` & `usau-scraper-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/docs/make.bat` & `usau-scraper-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/docs/source/conf.py` & `usau-scraper-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/docs/source/index.rst` & `usau-scraper-0.4.0/docs/source/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -2,59 +2,76 @@
    sphinx-quickstart on Sun Apr  2 21:26:33 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 usau-scraper documentation
 ===========================================
 
+.. image:: ../assets/project-logo.png
+  :width: 400
+  :align: center
+  :alt: USAU logo surrounded by gears
+
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    modules
+   developer
 
 Installation
 ===================================
-:code:`pip install usau-scraper`
+:code:`pip install --upgrade usau-scraper`
 
 How to Use
 ===================================
-After installing the library, there are currently 3 functions available for use:
-``getTeamInfo``, ``getTeamSchedule``, and ``getTeamRoster``.
-
-Simply :code:`import * from usau_scraper`, and get started!
+Simply :code:`from usau_scraper import *`, and get started!
 
 More extensive module documentation is here:
 :ref:`modules`
 
 Example Usage
 ===================================
 After :code:`pip install --upgrade usau-scraper` in your python env:
 
 ::
 
-   from usau_scraper import getTeamInfo, getTeamSchedule, getTeamRoster
+   from usau_scraper import *
 
    # Get a team's basic information
    print(getTeamInfo(
       schoolName = 'Columbia', 
       teamName = 'Baewatch', 
-      genderDivision=2, 
+      genderDivision='Women', 
       state='NY', 
       competitionLevel='College', 
-      competitionDivision=1, 
-      teamDesignation=1))
+      competitionDivision='Division 1', 
+      teamDesignation='B'))
 
    # Get a team's schedule for the current season
    print(getTeamSchedule(schoolName='Columbia', teamName='Curbside'))
 
    # Get a team's roster for the current season
    print(getTeamRoster(schoolName='Columbia', teamName='Curbside'))
 
+   # Get the pool play results for a tournament
+   print(getTournamentPoolPlayResults("College", "Women", eventName="No Sleep Till Brooklyn", season=2023))
+
+   # Get the bracket results for a tournament
+   print(getTournamentBracketResults("College", "Women", eventName="Centex", season=2022))
+
+   # Get the winner for a tournament
+   print(getTournamentWinner("College", "Women", eventName="Stanford Invite", season=2023))
+
+   # Get the top 20 women's college teams
+   print(getCollegeRankings(genderDivision="Women"))
+
+   # Get the top 20 women's club teams
+   print(getClubRankings(genderDivision="Women"))
+
 Additional usage examples are `in this notebook <https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb#scrollTo=rEfGbe_ruqk4>`_.
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
-* :ref:`search`
```

### Comparing `usau-scraper-0.3.0/examples/usau_scraper_example.ipynb` & `usau-scraper-0.4.0/examples/usau_scraper_example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995833333333333%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(9, "    genderDivision=\'Women\', \\n"), (12, "    '*

 * *            'competitionDivision=\'Division 1\', \\n"), (13, "    teamDesignation=\'B\'), '*

 * *            'indent=4))\\n"), (17, "    genderDivision=\'Women\', \\n")], delete: [17, 13, 12, '*

 * *            '9]}}}'}*

```diff
@@ -282,23 +282,23 @@
                 "# You can search for one specific team using schoolName and teamName\n",
                 "print(json.dumps(getTeamInfo(schoolName='Columbia', teamName='Curbside'), indent = 4))\n",
                 "\n",
                 "# Or search with even more specific information for a team (encodings will be made easier soon)\n",
                 "print(json.dumps(getTeamInfo(\n",
                 "    schoolName = 'Columbia', \n",
                 "    teamName = 'Baewatch', \n",
-                "    genderDivision=2, \n",
+                "    genderDivision='Women', \n",
                 "    state='NY', \n",
                 "    competitionLevel='College', \n",
-                "    competitionDivision=1, \n",
-                "    teamDesignation=1), indent=4))\n",
+                "    competitionDivision='Division 1', \n",
+                "    teamDesignation='B'), indent=4))\n",
                 "\n",
                 "# Search for the first 20 College Womens Teams in New York\n",
                 "print(json.dumps(getTeamInfo(\n",
-                "    genderDivision=2, \n",
+                "    genderDivision='Women', \n",
                 "    state='NY', \n",
                 "    competitionLevel='College'), indent=4))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
```

### Comparing `usau-scraper-0.3.0/pyproject.toml` & `usau-scraper-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "usau-scraper"
 authors = [{name = "Erin McNulty", email = "eem2188@columbia.edu"}]
 description="The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the USAU website."
 readme = "README.md"
-version = "0.3.0"
+version = "0.4.0"
 requires-python = ">=3.7"
 
 dependencies = ["bs4", "requests", "pandas", "lxml"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `usau-scraper-0.3.0/usau_scraper/teamScraper.py` & `usau-scraper-0.4.0/usau_scraper/teamScraper.py`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/usau_scraper/tests/test_all.py` & `usau-scraper-0.4.0/usau_scraper/tests/test_all.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 import requests
 from bs4 import BeautifulSoup
 
-from usau_scraper import queryTeam, getTeamRoster, getTeamInfo, getTeamSchedule, setArgs, fillInBasicInfo
+from usau_scraper import (
+    queryTeam,
+    getTeamRoster,
+    getTeamInfo,
+    getTeamSchedule,
+    setArgs,
+    fillInBasicInfo,
+    getTournamentBracketResults,
+    getTournamentPoolPlayResults,
+    getTournamentWinner,
+    getCollegeRankings,
+    getClubRankings,
+)
 
 # ------------------------------- UNIT TESTS -------------------------------
 
 
 # ------------------ queryTeam Tests ------------------
 def test_query_team_multiple_teams():
     team_results = queryTeam({"schoolName": "Columbia", "competitionLevel": "College", "genderDivision": "Women"})
@@ -169,7 +181,92 @@
         "position": "",
         "year": "College (GR)",
         "height": "5'5\"",
     }
 
     assert teams["res"] == "OK"
     assert expectedPlayer in teams["teams"][0]["roster"]
+
+
+# ------------------ getTournamentPoolPlayResults Tests ------------------
+def test_get_tournament_pool_play():
+    results = getTournamentPoolPlayResults("College", "Women", eventName="No Sleep Till Brooklyn", season=2023)
+
+    expectedPoolAResults = {
+        "Team": "Wellesley (1)",
+        "W - L": "3 - 0",
+    }
+
+    assert results["res"] == "OK"
+    del results["No Sleep Till Brooklyn 2023"]["pools"]["Pool A"][0]["Tie"]  # bc NaN != NaN
+    assert results["No Sleep Till Brooklyn 2023"]["pools"]["Pool A"][0] == expectedPoolAResults
+
+
+# ------------------ getTournamentBracketResults Tests ------------------
+def test_get_tournament_bracket():
+    results = getTournamentBracketResults("College", "Women", eventName="No Sleep Till Brooklyn", season=2023)
+
+    expectedFinalsResults = {
+        "date": "3/5/2023",
+        "time": "1:00PM",
+        "field": "8b",
+        "winner": "Wellesley (1)",
+        "loser": "Cornell (11)",
+        "score": "10 - 4",
+        "status": "Final",
+    }
+
+    assert results["res"] == "OK"
+    assert results["No Sleep Till Brooklyn 2023"]["Championship Bracket"]["Finals"][0] == expectedFinalsResults
+
+
+# ------------------ getTournamentWinner Tests ------------------
+def test_get_tournament_winner():
+    results = getTournamentWinner("College", "Women", eventName="No Sleep Till Brooklyn", season=2023)
+
+    expectedResults = {"firstPlace": "Wellesley (1)", "secondPlace": "Cornell (11)"}
+
+    assert results["res"] == "OK"
+    assert results["No Sleep Till Brooklyn 2023"] == expectedResults
+
+
+# ------------------ getCollegeRankings Tests ------------------
+def test_get_college_rankings():
+    teams = getCollegeRankings(genderDivision="Women")
+
+    expectedTeam = {
+        "Rank": "1",
+        "Team": "North Carolina",
+        "Power Rating": "2824",
+        "Competition Level": "College",
+        "Gender Division": "Women",
+        "Competition Division": "Division I",
+        "College Region": "Atlantic Coast",
+        "College Conference": "Carolina DI",
+        "Wins": "16",
+        "Losses": "0",
+    }
+
+    assert teams["res"] == "OK"
+    assert expectedTeam == teams["teams"][0]
+
+
+# ------------------ getClubRankings Tests ------------------
+def test_get_club_rankings():
+    teams = getClubRankings(genderDivision="Men")
+
+    expectedTeam = {
+        "Rank": "1",
+        "Team": "Truck Stop",
+        "Power Rating": "2134",
+        "Gender Division": "Men",
+        "Competition Division": "Pro",
+        "City": "Washington",
+        "State": "DC",
+        "Club Region": "Mid-Atlantic",
+        "Club Section": "Capital",
+        "Wins": "30",
+        "Losses": "4",
+    }
+
+    assert teams["res"] == "OK"
+    assert expectedTeam == teams["teams"][0]
```

### Comparing `usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/PKG-INFO` & `usau-scraper-0.4.0/usau_scraper/usau_scraper.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.3.0/usau_scraper.egg-info/PKG-INFO` & `usau-scraper-0.4.0/usau_scraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usau-scraper
-Version: 0.3.0
+Version: 0.4.0
 Summary: The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the USAU website.
 Author-email: Erin McNulty <eem2188@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,15 +217,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# USAU Scraper
+<p align="center">
+<img width="500" alt="USAU logo surrounded by data icons" src="https://user-images.githubusercontent.com/16248113/235183543-063d7200-5dcb-491d-bdbe-2eeaea6b5eee.png">
+</p>
 
 The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the [USAU website](https://play.usaultimate.org/events/tournament/?ViewAll=false&IsLeagueType=false&IsClinic=false&FilterByCategory=AE).
 
 ![Apache Liscence](https://img.shields.io/github/license/erin2722/usau-scraper?color=f72d2d)
 
 [![PyPI](https://img.shields.io/pypi/v/usau-scraper?color=2d2df7)](https://pypi.org/project/usau-scraper/)
 
@@ -238,160 +240,65 @@
 
 ## Overview
 
 USAU (USA Ultimate) is the governing body of ultimate frisbee, and its website (which is notoriously hard to navigate) contains all of the information about high school, college, and club ultimate frisbee teams. Right now, there is no easy way to access this data. USAU scraper solves this problem by scraping the USAU website for data and therefore allowing other developers to easily use the data on the USAU site. This project will open the door to more data analytic projects concerning ultimate frisbee.
 
 ## Installation
 
-`pip install usau-scraper`
-
-## How to Use
-
-After installing the library, there are currently 3 functions available for use: getTeamInfo, getTeamSchedule, and getTeamRoster.
-
-Simply `import * from usau_scraper`, and then call any of the following functions:
-
-### getTeamInfo()
-
-`getTeamInfo()` returns all information about the first 20 teams matching the query
-
-**Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
-
-**Output:**
-
-```
-{
-    res: OK, NOTFOUND
-    teams: [
-        {
-            schoolName,
-            teamName,
-            competitionLevel,
-            genderDivision,
-            location,
-            coaches,
-            website,
-            facebook,
-            twitter,
-        },
-        ...
-    ]
-}
-```
-
-### getTeamSchedule
-
-`getTeamSchedule()` returns the season schedule and record of the first 20 teams matching the query
-
-**Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
-
-**Output:**
-
-```
-{
-    res: OK, NOTFOUND
-    teams: [
-        {
-            schoolName,
-            teamName,
-            competitionLevel,
-            genderDivision,
-            wins,
-            losses,
-            tournaments: {
-                name: {
-                    games: [
-                        {
-                            date,
-                            score,
-                            opponentCollege,
-                            opponentTeamPage
-                        },
-                        ...
-                    ]
-                },
-                ...
-            },
-        },
-        ...
-    ]
-}
-```
-
-### getTeamRoster
-
-`getTeamRoster()` returns the roster of the first 20 teams matching the query
-
-**Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
-
-**Output:**
-
-```
-{
-    res: OK, NOTFOUND
-    teams: [
-        {
-            schoolName,
-            teamName,
-            competitionLevel,
-            genderDivision,
-            roster: [
-                {
-                    no,
-                    name,
-                    pronouns,
-                    position,
-                    year,
-                    height,
-                },
-                ...
-            ]
-        },
-        ...
-    ]
-}
-```
+`pip install --upgrade usau-scraper`
 
 ## Example Usage
 
-After `pip install --upgrade usau-scraper` in your python env:
-
 ```python
-from usau_scraper import getTeamInfo, getTeamSchedule, getTeamRoster
+from usau_scraper import *
 
 # Get a team's basic information
 print(getTeamInfo(
-    schoolName = 'Columbia', 
-    teamName = 'Baewatch', 
-    genderDivision=2, 
-    state='NY', 
-    competitionLevel='College', 
-    competitionDivision=1, 
-    teamDesignation=1))
+    schoolName = 'Columbia',
+    teamName = 'Baewatch',
+    genderDivision='Women',
+    state='NY',
+    competitionLevel='College',
+    competitionDivision='Division 1',
+    teamDesignation='B'))
 
 # Get a team's schedule for the current season
 print(getTeamSchedule(schoolName='Columbia', teamName='Curbside'))
 
 # Get a team's roster for the current season
 print(getTeamRoster(schoolName='Columbia', teamName='Curbside'))
+
+# Get the pool play results for a tournament
+print(getTournamentPoolPlayResults("College", "Women", eventName="No Sleep Till Brooklyn", season=2023))
+
+# Get the bracket results for a tournament
+print(getTournamentBracketResults("College", "Women", eventName="Centex", season=2022))
+
+# Get the winner for a tournament
+print(getTournamentWinner("College", "Women", eventName="Stanford Invite", season=2023))
+
+# Get the top 20 women's college teams
+print(getCollegeRankings(genderDivision="Women"))
+
+# Get the top 20 women's club teams
+print(getClubRankings(genderDivision="Women"))
 ```
 
 Additional usage examples are [in this notebook](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb#scrollTo=20Fjgtxr35ES).
 
 ## Features (MVP)
 
 - [x] A function that, given a team name, returns basic information about them.
 - [x] A function that, given a team name, returns their schedule and record.
 - [x] A function that, given a team name, returns its roster.
-- [ ] A function that, given a tournament name, returns the results of the tournament.
+- [x] A function that, given a tournament name, returns the results of the tournament.
 
 ## Additional features
 
-- [ ] A function that, given a college division, returns the current standings of that division.
-- [ ] An additional plugin to [frisbee-rankings.com](http://www.frisbee-rankings.com/) to show current top 25 teams.
+- [x] A function that, given a college division, returns the current standings of that division.
 - [ ] An additional plugin to ultiworld to show recent articles given a team name or college division.
 - [ ] More features tbd!
 
 ## Possible Applications
 
 - A seeding helper that, given a list of team names, returns their records for the season and their record against top 25 teams.
```

