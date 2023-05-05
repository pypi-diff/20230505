# Comparing `tmp/iso3166-2-1.0.1.tar.gz` & `tmp/iso3166-2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-2-1.0.1.tar", last modified: Thu May  4 21:48:53 2023, max compression
+gzip compressed data, was "iso3166-2-1.0.2.tar", last modified: Fri May  5 15:32:54 2023, max compression
```

## Comparing `iso3166-2-1.0.1.tar` & `iso3166-2-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.112526 iso3166-2-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-04 21:48:53.116526 iso3166-2-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.108526 iso3166-2-1.0.1/iso3166_2/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.108526 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1578148 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/iso3166-2-min.json
--rw-r--r--   0 runner    (1001) docker     (123)  3357755 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/iso3166-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.108526 iso3166-2-1.0.1/iso3166_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:48:51.000000 iso3166-2-1.0.1/iso3166_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-04 21:48:53.116526 iso3166-2-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.112526 iso3166-2-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/tests/test_iso3166_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:32:54.373752 iso3166-2-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-05 15:32:54.373752 iso3166-2-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:32:54.361752 iso3166-2-1.0.2/iso3166_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/iso3166_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:32:54.369752 iso3166-2-1.0.2/iso3166_2/iso3166-2-data/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/iso3166_2/iso3166-2-data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1578148 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/iso3166_2/iso3166-2-data/iso3166-2-min.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3357755 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/iso3166_2/iso3166-2-data/iso3166-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/iso3166_2/iso3166_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:32:54.365752 iso3166-2-1.0.2/iso3166_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-05 15:32:54.000000 iso3166-2-1.0.2/iso3166_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 15:32:54.000000 iso3166-2-1.0.2/iso3166_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:32:54.000000 iso3166-2-1.0.2/iso3166_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:32:53.000000 iso3166-2-1.0.2/iso3166_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 15:32:54.000000 iso3166-2-1.0.2/iso3166_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 15:32:54.000000 iso3166-2-1.0.2/iso3166_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-05 15:32:54.373752 iso3166-2-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:32:54.373752 iso3166-2-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-05-05 15:32:38.000000 iso3166-2-1.0.2/tests/test_iso3166_2.py
```

### Comparing `iso3166-2-1.0.1/LICENSE` & `iso3166-2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-2-1.0.1/PKG-INFO` & `iso3166-2-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-2
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 Home-page: https://github.com/amckenna41/iso3166-2
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
@@ -20,40 +20,42 @@
         <!-- [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR) -->
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
           <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
         </div>
         
-        > Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][demo].
+        > Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [here][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
-          * [Issues](#Issues)
+          * [Issues](#issuesorcontributing)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        <b>iso3166-2</b> is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
+        `iso3166-2` is a custom-built Python wrapper for the RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
         
         The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
         
+        The full list of attributes/fields available in `iso3166-2` can be viewed in the [ATTRIBUTES.md][attributes] file.
+        
         Latest Updates
         --------------
         An important thing to note about the ISO 3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a whole subdivision. Therefore, it's important that this library and its JSONs have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
         
-        The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
+        The <b>iso3166-updates</b> repo is another software package and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the <i>getISO3166_2.py</i> script is called regularly to check for any updates for all country data using the restcountries API. 
         
-        Installaion
-        -----------
+        Installation
+        ------------
         Install the latest version of `iso3166-2` via [PyPi][PyPi] using pip:
         
         ```bash
         pip3 install iso3166-2 --upgrade
         ```
         
         Installation from source:
@@ -67,17 +69,17 @@
         ------------
         * [python][python] >= 3.7
         * [requests][requests] >= 2.28.1
         * [iso3166][iso3166] >= 2.1.1
         
         Usage
         -----
-        There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
+        There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 subdivision data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
         
-        The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data run the `getISO3166_2.py` in a terminal or cmd, the script takes around 2 hours to execute (the script requires the additional pacakges: pycountry, tqdm and googlemaps):
+        The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data, run the `getISO3166_2.py` in a terminal or cmd below; (the script takes around 2 hours to execute):
         ```
         python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
         
         --json_filename: output filename for exported JSONs.
         --output_folder: output folder to store JSONs.
         ```
         
@@ -114,26 +116,22 @@
         
         canada_iso3166_2.subdivisions['CA-AB'] #Alberta subdivision
         denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
         estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
         fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
         ```
         
-        Attributes
-        ----------
-        You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the JSIN exports.
-        
         Issues or Contributing
         ----------------------
-        Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
+        Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year, the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
         
         Contact
         -------
-        If you have any questions or comments, please contact amckenna41@qub.ac.uk. <br><br>
-        [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
+        If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue in the [Issues][issues] tab.  <br><br>
+        <!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/) -->
         
         References
         ----------
         \[1\]: https://en.wikipedia.org/wiki/ISO_3166 <br>
         \[2\]: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
         
         Support
@@ -149,15 +147,15 @@
         [rest]: https://restcountries.com/
         [google-maps-api]: https://github.com/googlemaps/google-maps-services-python
         [PyPi]: https://pypi.org/project/iso3166-2/
         [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
         [demo]: https://colab.research.google.com/drive/1btfEx23bgWdkUPiwdwlDqKkmUp1S-_7U?usp=sharing
         [attributes]: https://github.com/amckenna41/iso3166-2/ATTRIBUTES.md 
         [issues]: https://github.com/amckenna41/iso3166-2/issues
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha2,iso3166-updates,rest countries
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha-2,iso3166-updates,rest countries
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `iso3166-2-1.0.1/README.md` & `iso3166-2-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,42 @@
 <!-- [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
   <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
-> Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][demo].
+> Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [here][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [Requirements](#requirements)
   * [Installation](#installation)
   * [Usage](#usage)
-  * [Issues](#Issues)
+  * [Issues](#issuesorcontributing)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-<b>iso3166-2</b> is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
+`iso3166-2` is a custom-built Python wrapper for the RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
 
 The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
 
+The full list of attributes/fields available in `iso3166-2` can be viewed in the [ATTRIBUTES.md][attributes] file.
+
 Latest Updates
 --------------
 An important thing to note about the ISO 3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a whole subdivision. Therefore, it's important that this library and its JSONs have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
 
-The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
+The <b>iso3166-updates</b> repo is another software package and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the <i>getISO3166_2.py</i> script is called regularly to check for any updates for all country data using the restcountries API. 
 
-Installaion
------------
+Installation
+------------
 Install the latest version of `iso3166-2` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-2 --upgrade
 ```
 
 Installation from source:
@@ -57,17 +59,17 @@
 ------------
 * [python][python] >= 3.7
 * [requests][requests] >= 2.28.1
 * [iso3166][iso3166] >= 2.1.1
 
 Usage
 -----
-There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
+There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 subdivision data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
 
-The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data run the `getISO3166_2.py` in a terminal or cmd, the script takes around 2 hours to execute (the script requires the additional pacakges: pycountry, tqdm and googlemaps):
+The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data, run the `getISO3166_2.py` in a terminal or cmd below; (the script takes around 2 hours to execute):
 ```
 python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
 
 --json_filename: output filename for exported JSONs.
 --output_folder: output folder to store JSONs.
 ```
 
@@ -104,26 +106,22 @@
 
 canada_iso3166_2.subdivisions['CA-AB'] #Alberta subdivision
 denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
 estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
 fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
 ```
 
-Attributes
-----------
-You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the JSIN exports.
-
 Issues or Contributing
 ----------------------
-Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
+Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year, the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
 
 Contact
 -------
-If you have any questions or comments, please contact amckenna41@qub.ac.uk. <br><br>
-[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
+If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue in the [Issues][issues] tab.  <br><br>
+<!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/) -->
 
 References
 ----------
 \[1\]: https://en.wikipedia.org/wiki/ISO_3166 <br>
 \[2\]: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 
 Support
```

### Comparing `iso3166-2-1.0.1/iso3166_2/iso3166-2-data/iso3166-2-min.json` & `iso3166-2-1.0.2/iso3166_2/iso3166-2-data/iso3166-2-min.json`

 * *Files identical despite different names*

### Comparing `iso3166-2-1.0.1/iso3166_2/iso3166-2-data/iso3166-2.json` & `iso3166-2-1.0.2/iso3166_2/iso3166-2-data/iso3166-2.json`

 * *Files identical despite different names*

### Comparing `iso3166-2-1.0.1/iso3166_2/iso3166_2.py` & `iso3166-2-1.0.2/iso3166_2/iso3166_2.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,83 +6,151 @@
 class ISO3166_2():
     """
     This class is used to access all the ISO-3166 and ISO-3166-2 country data and attributes.
     There are two JSON's available in the package, iso3166-2-min.json and iso3166-2.json. The 
     former is a minified JSON of all country's ISO3166-2 subdivision info including subdivision
     name, type, code, parent code, lat/longitude and URL to its flag (if applicable). The latter 
     contains a verbose collection of all country data pulled from the restcountries API as well 
-    as the country's subdivision data appened to each. Both JSONs are generated using the 
-    getISO3166_2.py script in the main directory. All of the keys and objects in the JSON are 
-    accessible via dot notation using the Map class.
+    as the country's subdivision data mentioned appened to each. Both JSONs are generated using 
+    the getISO3166_2.py script in the main directory. All of the keys and objects in the JSON 
+    are accessible via dot notation using the Map class. The plethora of attributes available
+    in this class are described in the ATTRIBUTES.md file on the main repo dir 
+    (https://github.com/amckenna41/iso3166-2/blob/main/ATTRIBUTES.md).
     
     Parameters
     ----------
     : iso3166_json_filename : str (default=iso3166-2-min.json)
         filename of iso3166-2 JSON data to import from data folder. Can either be the
         iso3166-2-min or iso3166-2 JSON files. 
 
     Usage
     -----
     import iso3166_2 as iso
 
-    #get all country data for Ireland, Colombia, Denmark and Finland
+    #get ALL country data (including subdivision data) for Ireland, Colombia, Denmark and Finland
     iso.country['IE']
     iso.country['CO']
     iso.country['DK']
     iso.country['FI']
 
     #get capital city, languages, region and currency for Morocco
     iso.country['MA'].capital
     iso.country['MA'].languages
     iso.country['MA'].region
     iso.country['MA'].currencies
 
-    #get all subdivision data for Lithuania
+    #get ALL subdivision data for Lithuania, Namibia, Paraguay and Turkmenistan
     iso.subdivisions['LT'].subdivisions
-
-    #get subdivision names and subdivision types for GB-ANS, GB-BPL, GB-NTH and GB-WGN codes for the UK
-    iso.subdivisions['GB'].subdivisions['GB-ANS].name
+    iso.subdivisions['NA'].subdivisions
+    iso.subdivisions['PY'].subdivisions
+    iso.subdivisions['TM'].subdivisions
+
+    #get subdivision names, types, parent codes, flag urls and lat/longitudes 
+    #for GB-ANS, GB-BPL, GB-NTH, GB-WGN and GB-ZET subdivision codes for the UK
+    iso.subdivisions['GB'].subdivisions['GB-ANS'].name
+    iso.subdivisions['GB'].subdivisions['GB-BPL'].type
+    iso.subdivisions['GB'].subdivisions['GB-NTH'].parent_code
+    iso.subdivisions['GB'].subdivisions['GB-WGN'].flag_url
+    iso.subdivisions['GB'].subdivisions['GB-ZET'].latlng
     """
     def __init__(self, iso3166_json_filename="iso3166-2-min.json"):
 
         self.iso3166_json_filename= iso3166_json_filename
         self.data_folder = "iso3166-2-data"
+        self.using_country_data = False
+        self.using_subdivision_data = False
 
         #get module path
         self.iso3166_2_module_path = os.path.dirname(os.path.abspath(sys.modules[self.__module__].__file__))
         
         #raise error if iso3166-2 json doesnt exist in the data folder
         if not (os.path.isfile(os.path.join(self.iso3166_2_module_path, self.data_folder, self.iso3166_json_filename))):
             raise OSError("Issue finding iso3166-2.json in data dir {}.".format(self.data_folder))
 
         #open iso3166-2 json file and load it into class variable
         with open(os.path.join(self.iso3166_2_module_path, self.data_folder, self.iso3166_json_filename)) as iso3166_2_json:
             self.all_iso3166_2_data = json.load(iso3166_2_json)
         
+        #set bool variables indicating which json is being used
+        if (self.iso3166_json_filename == "iso3166-2-min.json"):
+            self.using_subdivision_data = True
+        elif (self.iso3166_json_filename == "iso3166-2.json"):
+            self.using_country_data = True
+
         #get list of all countries by 2 letter alpha3 code
         self.alpha2 = sorted(list(iso3166.countries_by_alpha2.keys()))
         
         #get list of all countries by 3 letter alpha3 code
         self.alpha3 = sorted(list(iso3166.countries_by_alpha3.keys()))
-    
-    def __sizeof__(self):
-        """ Return size of instance of ISO3166-2 class. """
-        return self.__sizeof__()
+
+    def subdivision_codes(self, alpha2_code):
+        """
+        Return a list of all ISO3166-2 subdivision codes for country specified by
+        its 2 letter alpha-2 code.
+
+        Parameters
+        ----------
+        : alpha2_code: str
+            2 letter ISO3166-1 alpha-2 code for country.
+        
+        Returns
+        -------
+        : list 
+            list of a country's ISO3166-2 subdivision codes.
+        """
+        #raise error if invalid alpha-2 code input to func
+        if not (alpha2_code in sorted(list(iso3166.countries_by_alpha2.keys()))):
+            raise ValueError("Invalid alpha-2 code input: {}.".format(alpha2_code))
+
+        #return list of subdivision codes, get current JSON being used in class, the 2 JSONs have different nested dicts
+        if (self.using_country_data):
+            return list(self.all_iso3166_2_data[alpha2_code]["subdivisions"])
+        else:
+            return list(self.all_iso3166_2_data[alpha2_code])
+
+        return list(self.all_iso3166_2_data[alpha2_code])
+
+    def subdivision_names(self, alpha2_code):
+        """
+        Return a list of all ISO3166-2 subdivision names for country specified by
+        its 2 letter alpha-2 code.
+
+        Parameters
+        ----------
+        : alpha2_code: str
+            2 letter ISO3166-1 alpha-2 code for country.
+        
+        Returns
+        -------
+        : list 
+            list of a country's ISO3166-2 subdivision names.
+        """
+        #raise error if invalid alpha-2 code input to func
+        if not (alpha2_code in sorted(list(iso3166.countries_by_alpha2.keys()))):
+            raise ValueError("Invalid alpha-2 code input: {}.".format(alpha2_code))
+
+        #return list of subdivision names, get current JSON being used in class, the 2 JSONs have different nested dicts
+        if (self.using_country_data):
+            return [self.all_iso3166_2_data[alpha2_code]["subdivisions"][x]["name"] for x in self.all_iso3166_2_data[alpha2_code]["subdivisions"]]
+        else:
+            return [self.all_iso3166_2_data[alpha2_code][x]["name"] for x in self.all_iso3166_2_data[alpha2_code]]
 
     def __getitem__(self, alpha2_code):
         """
         Return all of a countrys data and subdivision by making the class
-        subscriptable. The 2 letter alpha2 code is expected as input, 
-        although the 3 letter alpha3 code can be input which will be 
-        converted into its alpha2 counterpart.
+        subscriptable. The 2 letter alpha-2 code is expected as input, 
+        although, for redundancy, the 3 letter alpha-3 code can be input 
+        which will be converted into its alpha-2 counterpart.
 
         Parameters
         ----------
         : alpha2_code : str
-            2 letter alpha2 code for sought country/territory e.g (AD, EG, DE).
+            2 letter alpha-2 code for sought country/territory e.g (AD, EG, DE).
+            Can also accept 3 letter alpha-3 code e.g (AND, EGT, DEU), this will 
+            be converted into its alpha-2 counterpart.
 
         Returns
         -------
         : country[alpha2_code]: dict
             dict object of country/subdivision info for inputted alpha2_code.
 
         Usage
@@ -111,27 +179,25 @@
         
         #stripping input of whitespace and uppercasing
         alpha2_code = alpha2_code.strip().upper()
 
         #object to store country data
         country = {}
 
-        #validate 2 letter alpha2 code exists in ISO3166-1, raise error if not found            
+        #validate 2 letter alpha-2 code exists in ISO3166-1, raise error if not found            
         if (len(alpha2_code) == 2):
-            if (alpha2_code in self.alpha2):      
-                alpha2_code = iso3166.countries_by_alpha2[alpha2_code].alpha2
-            else:
-                raise ValueError("Alpha2 Code {} not found in list of ISO3166-1 codes.".format(alpha2_code))            
+            if not (alpha2_code in self.alpha2):      
+                raise ValueError("Alpha-2 Code {} not found in list of ISO3166-1 codes.".format(alpha2_code))            
         
-        #if 3 letter code input, check it exists in ISO3166-1, then convert into its 2 letter alpha2 code, raise error if not found            
+        #if 3 letter code input, check it exists in ISO3166-1, then convert into its 2 letter alpha-2 code, raise error if not found            
         if (len(alpha2_code) == 3):
             if (alpha2_code in self.alpha3):      
                 alpha2_code = iso3166.countries_by_alpha3[alpha2_code].alpha2
             else:
-                raise ValueError("Alpha3 Code {} not found in list of ISO3166-1 codes.".format(alpha2_code))            
+                raise ValueError("Alpha-3 Code {} not found in list of ISO3166-1 codes.".format(alpha2_code))            
 
         #create instance of Map class so dict can be accessed via dot notation 
         country[alpha2_code] = Map(self.all_iso3166_2_data[alpha2_code]) 
 
         #iterate over nested dicts, convert into instances of Map class so they can be accessed via dot notation
         for key in country[alpha2_code].keys():
             if (isinstance(country[alpha2_code][key], dict)):
@@ -141,14 +207,18 @@
         country = Map(country)
                  
         return country[alpha2_code]
 
     def __str__(self):
         return "Instance of ISO3166-2 class."
 
+    def __sizeof__(self):
+        """ Return size of instance of ISO3166-2 class. """
+        return self.__sizeof__()
+
 class Map(dict):
     """
     Class that accepts a dict and allows you to use dot notation to access
     members of the dictionary. 
 
     Parameters
     ----------
@@ -172,15 +242,14 @@
     del m.new_key
     # Or
     del m['new_key']
 
     References
     ----------
     [1]: https://stackoverflow.com/questions/2352181/how-to-use-a-dot-to-access-members-of-dictionary
-
     """
     def __init__(self, *args, **kwargs):
         super(Map, self).__init__(*args, **kwargs)
         for arg in args:
             if isinstance(arg, dict):
                 for k, v in arg.items():
                     self[k] = v
```

### Comparing `iso3166-2-1.0.1/iso3166_2.egg-info/PKG-INFO` & `iso3166-2-1.0.2/iso3166_2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-2
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 Home-page: https://github.com/amckenna41/iso3166-2
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
@@ -20,40 +20,42 @@
         <!-- [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR) -->
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
           <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
         </div>
         
-        > Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][demo].
+        > Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [here][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
-          * [Issues](#Issues)
+          * [Issues](#issuesorcontributing)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        <b>iso3166-2</b> is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
+        `iso3166-2` is a custom-built Python wrapper for the RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
         
         The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
         
+        The full list of attributes/fields available in `iso3166-2` can be viewed in the [ATTRIBUTES.md][attributes] file.
+        
         Latest Updates
         --------------
         An important thing to note about the ISO 3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a whole subdivision. Therefore, it's important that this library and its JSONs have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
         
-        The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
+        The <b>iso3166-updates</b> repo is another software package and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the <i>getISO3166_2.py</i> script is called regularly to check for any updates for all country data using the restcountries API. 
         
-        Installaion
-        -----------
+        Installation
+        ------------
         Install the latest version of `iso3166-2` via [PyPi][PyPi] using pip:
         
         ```bash
         pip3 install iso3166-2 --upgrade
         ```
         
         Installation from source:
@@ -67,17 +69,17 @@
         ------------
         * [python][python] >= 3.7
         * [requests][requests] >= 2.28.1
         * [iso3166][iso3166] >= 2.1.1
         
         Usage
         -----
-        There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
+        There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 subdivision data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
         
-        The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data run the `getISO3166_2.py` in a terminal or cmd, the script takes around 2 hours to execute (the script requires the additional pacakges: pycountry, tqdm and googlemaps):
+        The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data, run the `getISO3166_2.py` in a terminal or cmd below; (the script takes around 2 hours to execute):
         ```
         python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
         
         --json_filename: output filename for exported JSONs.
         --output_folder: output folder to store JSONs.
         ```
         
@@ -114,26 +116,22 @@
         
         canada_iso3166_2.subdivisions['CA-AB'] #Alberta subdivision
         denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
         estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
         fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
         ```
         
-        Attributes
-        ----------
-        You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the JSIN exports.
-        
         Issues or Contributing
         ----------------------
-        Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
+        Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year, the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
         
         Contact
         -------
-        If you have any questions or comments, please contact amckenna41@qub.ac.uk. <br><br>
-        [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
+        If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue in the [Issues][issues] tab.  <br><br>
+        <!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/) -->
         
         References
         ----------
         \[1\]: https://en.wikipedia.org/wiki/ISO_3166 <br>
         \[2\]: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
         
         Support
@@ -149,15 +147,15 @@
         [rest]: https://restcountries.com/
         [google-maps-api]: https://github.com/googlemaps/google-maps-services-python
         [PyPi]: https://pypi.org/project/iso3166-2/
         [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
         [demo]: https://colab.research.google.com/drive/1btfEx23bgWdkUPiwdwlDqKkmUp1S-_7U?usp=sharing
         [attributes]: https://github.com/amckenna41/iso3166-2/ATTRIBUTES.md 
         [issues]: https://github.com/amckenna41/iso3166-2/issues
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha2,iso3166-updates,rest countries
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha-2,iso3166-updates,rest countries
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `iso3166-2-1.0.1/setup.cfg` & `iso3166-2-1.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-2
-version = 1.0.1
+version = 1.0.2
 description = A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/amckenna41/iso3166-2
 download_url = https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
@@ -16,15 +16,15 @@
 	beautifulsoup
 	python
 	pypi
 	countries
 	country codes
 	iso3166-2
 	iso3166-1
-	alpha2
+	alpha-2
 	iso3166-updates
 	rest-countries
 classifiers = 
 	Development Status :: 3 - Alpha,
 	Environment :: Console,
 	Intended Audience :: Developers,
 	Intended Audience :: Science/Research,
```

### Comparing `iso3166-2-1.0.1/setup.py` & `iso3166-2-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-2'
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __description__ = "A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __maintainer__ = "AJ McKenna"
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-2'
 __download_url__ = "https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip"
 __status__ = 'Development'
 __keywords__ = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", \
-            "iso3166-2", "iso3166-1", "alpha2", "iso3166-updates", "rest countries"]
+            "iso3166-2", "iso3166-1", "alpha-2", "iso3166-updates", "rest countries"]
 __test_suite__ = "tests"
 
 #ensure python version is greater than 3
 if (sys.version_info[0] < 3):
     sys.exit('Python 3 is the minimum version requirement.')
 
 #get path to README file
@@ -59,14 +59,13 @@
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
       install_requires=[
           'requests>=2.28.1',
-          'iso3166',
-          'googlemaps'
+          'iso3166'
       ],
      test_suite=__test_suite__,
      packages=find_packages(),
      include_package_data=True,
      zip_safe=False)
```

### Comparing `iso3166-2-1.0.1/tests/test_iso3166_2.py` & `iso3166-2-1.0.2/tests/test_iso3166_2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import iso3166_2 as iso
 import iso3166
 import requests
 import json
 import os
 import getpass
-from importlib import metadata
-try:
-    from importlib import metadata
-except ImportError:
-    import importlib_metadata as metadata  
+# import importlib.metadata as metadata  
 import unittest
 unittest.TestLoader.sortTestMethodsUsing = None
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 class ISO3166_2_Updates(unittest.TestCase):
 
     def setUp(self):
         """ Initialise test variables, import json. """
         #initalise User-agent header for requests library 
         self.user_agent_header = {'User-Agent': 'iso3166-2/{} ({}; {})'.format(__version__,
@@ -29,70 +25,70 @@
         #import min iso3166-2 json
         with open(os.path.join("iso3166_2", "iso3166-2-data", "iso3166-2-min.json")) as iso3166_2_json:
             self.all_iso3166_2_min_data = json.load(iso3166_2_json)
 
         #base url for flag icons on iso3166-flag-icons repo
         self.flag_icons_base_url = "https://github.com/amckenna41/iso3166-flag-icons/blob/main/iso3166-2-icons/"
 
-    @unittest.skip("")
-    def test_iso3166_2_metadata(self): 
-        """ Testing correct iso3166-2 software version and metadata. """
-        self.assertEqual(metadata.metadata('iso3166-2')['version'], "1.0.1", 
-            "iso3166-2 version is not correct, got: {}".format(metadata.metadata('iso3166-2')['version']))
-        self.assertEqual(metadata.metadata('iso3166-2')['name'], "iso3166-2", 
-            "iso3166-2 software name is not correct, got: {}".format(metadata.metadata('iso3166-2')['name']))
-        self.assertEqual(metadata.metadata('iso3166-2')['author'], 
-            "AJ McKenna, https://github.com/amckenna41", "iso3166-updates author is not correct, got: {}".format(metadata.metadata('iso3166_2')['author']))
-        self.assertEqual(metadata.metadata('iso3166-2')['author-email'], 
-            "amckenna41@qub.ac.uk", "iso3166-updates author email is not correct, got: {}".format(metadata.metadata('iso3166_2')['author-email']))
-        self.assertEqual(metadata.metadata('iso3166-2')['keywords'], 
-            ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "iso3166-2", "iso3166-1", "alpha2", "iso3166-updates", "rest countries"], 
-                "iso3166-updates keywords are not correct, got: {}".format(metadata.metadata('iso3166-2')['keywords']))
-        self.assertEqual(metadata.metadata('iso3166-2')['home-page'], 
-            "https://github.com/amckenna41/iso3166-updates", "iso3166-updates home page url is not correct, got: {}".format(metadata.metadata('iso3166_2')['home-page']))
-        self.assertEqual(metadata.metadata('iso3166-2')['maintainer'], 
-            "AJ McKenna", "iso3166-updates maintainer is not correct, got: {}".format(metadata.metadata('iso3166-2')['maintainer']))
-        self.assertEqual(metadata.metadata('iso3166-2')['license'], "MIT", 
-            "iso3166-updates license type is not correct, got: {}".format(metadata.metadata('iso3166-2')['license']))
+    # @unittest.skip("")
+    # def test_iso3166_2_metadata(self): 
+    #     """ Testing correct iso3166-2 software version and metadata. """
+    #     self.assertEqual(metadata.metadata('iso3166_2')['version'], "1.0.2", 
+    #         "iso3166-2 version is not correct, got: {}".format(metadata.metadata('iso3166-2')['version']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['name'], "iso3166-2", 
+    #         "iso3166-2 software name is not correct, got: {}".format(metadata.metadata('iso3166-2')['name']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['author'], 
+    #         "AJ McKenna, https://github.com/amckenna41", "iso3166-updates author is not correct, got: {}".format(metadata.metadata('iso3166_2')['author']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['author-email'], 
+    #         "amckenna41@qub.ac.uk", "iso3166-updates author email is not correct, got: {}".format(metadata.metadata('iso3166_2')['author-email']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['keywords'], 
+    #         ','.join(["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "iso3166-2", "iso3166-1", "alpha-2", "iso3166-updates", "rest countries"]).replace(" ", ""), 
+    #             "iso3166-updates keywords are not correct, got: {}".format(metadata.metadata('iso3166-2')['keywords']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['home-page'], 
+    #         "https://github.com/amckenna41/iso3166-2", "iso3166-2 home page url is not correct, got: {}".format(metadata.metadata('iso3166_2')['home-page']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['maintainer'], 
+    #         "AJ McKenna", "iso3166-updates maintainer is not correct, got: {}".format(metadata.metadata('iso3166-2')['maintainer']))
+    #     self.assertEqual(metadata.metadata('iso3166-2')['license'], "MIT", 
+    #         "iso3166-updates license type is not correct, got: {}".format(metadata.metadata('iso3166-2')['license']))
 
     def test_iso3166_2(self):
         """ Test ISO3166-2 class and its methods and attributes. """
         #testing class using iso3166-2.json file as input
         self.assertIsInstance(iso.country.alpha2, list, 
-            "Expected alpha2 attribute to be a list, got {}.".format(type(iso.country.alpha2)))
+            "Expected alpha-2 attribute to be a list, got {}.".format(type(iso.country.alpha2)))
         self.assertEqual(len(iso.country.alpha2), 250, 
-            "Expected 250 alpha2 codes, got {}.".format(len(iso.country.alpha2)))
+            "Expected 250 alpha-2 codes, got {}.".format(len(iso.country.alpha2)))
         self.assertIsInstance(iso.country.alpha3, list, 
             "Expected alpha3 attribute to be a list, got {}.".format(type(iso.country.alpha3)))
         self.assertEqual(len(iso.country.alpha3), 250, 
             "Expected 250 alpha3 codes, got {}.".format(len(iso.country.alpha3)))
         self.assertIsInstance(iso.country.all_iso3166_2_data, dict,
             "Expected ISO3166-2 data object to be a dict, got {}.".format(type(iso.country.all_iso3166_2_data)))
         self.assertEqual(len(iso.country.all_iso3166_2_data), 250, 
             "Expected 250 countrys in ISO3166-2 data object, got {}.".format(len(iso.country.all_iso3166_2_data)))       
         for code in iso.country.all_iso3166_2_data:
             self.assertIn(code, iso.country.alpha2,
-                "Alpha2 code {} not found in list of available 2 letter codes.".format(code))
+                "Alpha-2 code {} not found in list of available 2 letter codes.".format(code))
 
         #testing class using iso3166-2-min.json file as input
         self.assertIsInstance(iso.subdivisions.alpha2, list, 
-            "Expected alpha2 attribute to be a list, got {}.".format(type(iso.subdivisions.alpha2)))
+            "Expected alpha-2 attribute to be a list, got {}.".format(type(iso.subdivisions.alpha2)))
         self.assertEqual(len(iso.subdivisions.alpha2), 250, 
-            "Expected 250 alpha2 codes, got {}.".format(len(iso.subdivisions.alpha2)))
+            "Expected 250 alpha-2 codes, got {}.".format(len(iso.subdivisions.alpha2)))
         self.assertIsInstance(iso.subdivisions.alpha3, list, 
             "Expected alpha3 attribute to be a list, got {}.".format(type(iso.country.alpha3)))
         self.assertEqual(len(iso.subdivisions.alpha3), 250, 
             "Expected 250 alpha3 codes, got {}.".format(len(iso.subdivisions.alpha3)))
         self.assertIsInstance(iso.subdivisions.all_iso3166_2_data, dict,
             "Expected ISO3166-2 data object to be a dict, got {}.".format(type(iso.subdivisions.all_iso3166_2_data)))
         self.assertEqual(len(iso.subdivisions.all_iso3166_2_data), 250, 
             "Expected 250 countrys in ISO3166-2 data object, got {}.".format(len(iso.subdivisions.all_iso3166_2_data)))       
         for code in iso.subdivisions.all_iso3166_2_data:
             self.assertIn(code, iso.subdivisions.alpha2,
-                "Alpha2 code {} not found in list of available 2 letter codes.".format(code))
+                "Alpha-2 code {} not found in list of available 2 letter codes.".format(code))
         
     def test_iso3166_2_json(self):
         """ Testing iso3166-2.json contents and data. """
         test_alpha2_au = iso.country['AU'] #Australia
         test_alpha2_lu = iso.country['LU'] #Luxembourg
         test_alpha2_mg = iso.country["MG"] #Madagascar 
         test_alpha2_om = iso.country["OM"] #Oman
@@ -106,60 +102,60 @@
         self.assertEqual(test_alpha2_au.capital[0], "Canberra")        
         self.assertEqual(test_alpha2_au.region, "Oceania")        
         self.assertEqual(list(test_alpha2_au.languages.keys())[0], "eng")        
         self.assertEqual(test_alpha2_au.area, 7692024)        
         self.assertEqual(test_alpha2_au.population, 25687041)        
         self.assertEqual(test_alpha2_au.latlng, [-27.0, 133.0], "")        
         self.assertEqual(len(test_alpha2_au.subdivisions), 8, "")
-        self.assertEqual(test_alpha2_au, iso.country['AUS']) #test objects match if using either alpha2/alpha3 codes
+        self.assertEqual(test_alpha2_au, iso.country['AUS']) #test objects match if using either alpha-2/alpha-3 codes
 #2.)
         self.assertIsInstance(test_alpha2_lu, dict, "")
         self.assertEqual(len(test_alpha2_lu), 36, "")
         self.assertEqual(test_alpha2_lu.name.common, "Luxembourg")        
         self.assertEqual(test_alpha2_lu.cca2, "LU")        
         self.assertEqual(test_alpha2_lu.cca3, "LUX")        
         self.assertEqual(test_alpha2_lu.currencies.EUR['name'], "Euro")        
         self.assertEqual(test_alpha2_lu.capital[0], "Luxembourg")        
         self.assertEqual(test_alpha2_lu.region, "Europe")        
         self.assertEqual(list(test_alpha2_lu.languages.keys()), ["deu", "fra", "ltz"])        
         self.assertEqual(test_alpha2_lu.area, 2586)        
         self.assertEqual(test_alpha2_lu.population, 632275)        
         self.assertEqual(len(test_alpha2_lu.subdivisions), 12, "")
         self.assertEqual(test_alpha2_lu.latlng, [49.75, 6.16666666], "")        
-        self.assertEqual(test_alpha2_lu, iso.country['LUX']) #test objects match if using either alpha2/alpha3 codes
+        self.assertEqual(test_alpha2_lu, iso.country['LUX']) #test objects match if using either alpha-2/alpha-3 codes
 #3.)
         self.assertIsInstance(test_alpha2_mg, dict, "")
         self.assertEqual(len(test_alpha2_mg), 35, "")
         self.assertEqual(test_alpha2_mg.name.common, "Madagascar")        
         self.assertEqual(test_alpha2_mg.cca2, "MG")        
         self.assertEqual(test_alpha2_mg.cca3, "MDG")        
         self.assertEqual(test_alpha2_mg.currencies.MGA['name'], "Malagasy ariary")        
         self.assertEqual(test_alpha2_mg.capital[0], "Antananarivo")        
         self.assertEqual(test_alpha2_mg.region, "Africa")        
         self.assertEqual(list(test_alpha2_mg.languages.keys()), ["fra", "mlg"])        
         self.assertEqual(test_alpha2_mg.area, 587041)        
         self.assertEqual(test_alpha2_mg.population, 27691019)        
         self.assertEqual(test_alpha2_mg.latlng, [-20.0, 47.0], "")        
         self.assertEqual(len(test_alpha2_mg.subdivisions), 6, "")
-        self.assertEqual(test_alpha2_mg, iso.country['MDG']) #test objects match if using either alpha2/alpha3 codes
+        self.assertEqual(test_alpha2_mg, iso.country['MDG']) #test objects match if using either alpha-2/alpha-3 codes
 #4.)
         self.assertIsInstance(test_alpha2_om, dict, "")
         self.assertEqual(len(test_alpha2_om), 35, "")
         self.assertEqual(test_alpha2_om.name.common, "Oman")        
         self.assertEqual(test_alpha2_om.cca2, "OM")        
         self.assertEqual(test_alpha2_om.cca3, "OMN")        
         self.assertEqual(test_alpha2_om.currencies.OMR['name'], "Omani rial")        
         self.assertEqual(test_alpha2_om.capital[0], "Muscat")        
         self.assertEqual(test_alpha2_om.region, "Asia")        
         self.assertEqual(list(test_alpha2_om.languages.keys()), ["ara"])        
         self.assertEqual(test_alpha2_om.area, 309500)        
         self.assertEqual(test_alpha2_om.population, 5106622)        
         self.assertEqual(test_alpha2_om.latlng, [21.0, 57.0], "")        
         self.assertEqual(len(test_alpha2_om.subdivisions), 11, "")
-        self.assertEqual(test_alpha2_om, iso.country['OMN']) #test objects match if using either alpha2/alpha3 codes
+        self.assertEqual(test_alpha2_om, iso.country['OMN']) #test objects match if using either alpha-2/alpha-3 codes
 #5.)
         with (self.assertRaises(ValueError)):
             invalid_country = iso.country["ZZ"]
             invalid_country = iso.country["XY"]
             invalid_country = iso.country["XYZ"]
 #6.)
         with (self.assertRaises(TypeError)):
@@ -234,14 +230,88 @@
             invalid_country = iso.subdivisions["XYZ"]
 #6.)
         with (self.assertRaises(TypeError)):
             invalid_country = iso.subdivisions[123]
             invalid_country = iso.subdivisions[0.5]
             invalid_country = iso.subdivisions[False]
 
+    def test_subdivision_names(self):
+        """ Testing functionality for getting list of all ISO3166-2 subdivision names. """
+        expected_km_subdivision_names = ['Andjouân', 'Andjazîdja', 'Mohéli']
+        expected_er_subdivision_names = ['Ansabā', 'Debubawi K’eyyĭḥ Baḥri', 'Al Janūbī', 'Gash-Barka', 'Al Awsaţ', 'Semienawi K’eyyĭḥ Baḥri']
+        expected_gl_subdivision_names = ['Avannaata Kommunia', 'Kommune Kujalleq', 'Qeqqata Kommunia', 'Kommune Qeqertalik', 'Kommuneqarfik Sermersooq']
+        expected_vc_subdivision_names = ['Charlotte', 'Saint Andrew', 'Saint David', 'Saint George', 'Saint Patrick', 'Grenadines']
+#1.)        
+        km_subdivision_names = iso.subdivisions.subdivision_names("KM") #Comoros
+        er_subdivision_names = iso.subdivisions.subdivision_names("ER") #Eritrea
+        gl_subdivision_names = iso.subdivisions.subdivision_names("GL") #Greenland
+        vc_subdivision_names = iso.subdivisions.subdivision_names("VC") #St Vincent
+
+        self.assertEqual(km_subdivision_names, expected_km_subdivision_names, "")
+        self.assertEqual(er_subdivision_names, expected_er_subdivision_names, "")
+        self.assertEqual(gl_subdivision_names, expected_gl_subdivision_names, "")
+        self.assertEqual(vc_subdivision_names, expected_vc_subdivision_names, "")
+
+        self.assertIsInstance(km_subdivision_names, list, "")
+        self.assertIsInstance(er_subdivision_names, list, "")
+        self.assertIsInstance(gl_subdivision_names, list, "")
+        self.assertIsInstance(vc_subdivision_names, list, "")
+#2.)   
+        km_subdivision_names = iso.country.subdivision_names("KM") #Comoros
+        er_subdivision_names = iso.country.subdivision_names("ER") #Eritrea
+        gl_subdivision_names = iso.country.subdivision_names("GL") #Greenland
+        vc_subdivision_names = iso.country.subdivision_names("VC") #St Vincent
+
+        self.assertEqual(km_subdivision_names, expected_km_subdivision_names, "")
+        self.assertEqual(er_subdivision_names, expected_er_subdivision_names, "")
+        self.assertEqual(gl_subdivision_names, expected_gl_subdivision_names, "")
+        self.assertEqual(vc_subdivision_names, expected_vc_subdivision_names, "")
+
+        self.assertIsInstance(km_subdivision_names, list, "")
+        self.assertIsInstance(er_subdivision_names, list, "")
+        self.assertIsInstance(gl_subdivision_names, list, "")
+        self.assertIsInstance(vc_subdivision_names, list, "")
+
+    def test_subdivision_codes(self):
+        """ Testing functionality for getting list of all ISO3166-2 subdivision codes. """
+        expected_bq_subdivision_codes = ['BQ-BO', 'BQ-SA', 'BQ-SE']
+        expected_sz_subdivision_codes = ['SZ-HH', 'SZ-LU', 'SZ-MA', 'SZ-SH']
+        expected_sm_subdivision_codes = ['SM-01', 'SM-02', 'SM-03', 'SM-04', 'SM-05', 'SM-06', 'SM-07', 'SM-08', 'SM-09']
+        expected_wf_subdivision_codes = ['WF-AL', 'WF-SG', 'WF-UV']
+#1.)        
+        bq_subdivision_codes = iso.subdivisions.subdivision_codes("BQ") #Bonaire, Sint Eustatius and Saba
+        sz_subdivision_codes = iso.subdivisions.subdivision_codes("SZ") #Eswatini
+        sm_subdivision_codes = iso.subdivisions.subdivision_codes("SM") #San Marino
+        wf_subdivision_codes = iso.subdivisions.subdivision_codes("WF") #Wallace and Futuna 
+
+        self.assertEqual(bq_subdivision_codes, expected_bq_subdivision_codes, "")
+        self.assertEqual(sz_subdivision_codes, expected_sz_subdivision_codes, "")
+        self.assertEqual(sm_subdivision_codes, expected_sm_subdivision_codes, "")
+        self.assertEqual(wf_subdivision_codes, expected_wf_subdivision_codes, "")
+
+        self.assertIsInstance(bq_subdivision_codes, list, "")
+        self.assertIsInstance(sz_subdivision_codes, list, "")
+        self.assertIsInstance(sm_subdivision_codes, list, "")
+        self.assertIsInstance(wf_subdivision_codes, list, "")
+#2.)   
+        bq_subdivision_codes = iso.country.subdivision_codes("BQ") #Bonaire, Sint Eustatius and Saba
+        sz_subdivision_codes = iso.country.subdivision_codes("SZ") #Eswatini
+        sm_subdivision_codes = iso.country.subdivision_codes("SM") #San Marino
+        wf_subdivision_codes = iso.country.subdivision_codes("WF") #Wallace and Futuna 
+
+        self.assertEqual(bq_subdivision_codes, expected_bq_subdivision_codes, "")
+        self.assertEqual(sz_subdivision_codes, expected_sz_subdivision_codes, "")
+        self.assertEqual(sm_subdivision_codes, expected_sm_subdivision_codes, "")
+        self.assertEqual(wf_subdivision_codes, expected_wf_subdivision_codes, "")
+
+        self.assertIsInstance(bq_subdivision_codes, list, "")
+        self.assertIsInstance(sz_subdivision_codes, list, "")
+        self.assertIsInstance(sm_subdivision_codes, list, "")
+        self.assertIsInstance(wf_subdivision_codes, list, "")
+
     def tearDown(self):
         """ Delete all iso3166-2 json objects or instances. """
         del self.all_iso3166_2_data
         del self.all_iso3166_2_min_data
     
 if __name__ == '__main__':
     #run all unit tests
```

