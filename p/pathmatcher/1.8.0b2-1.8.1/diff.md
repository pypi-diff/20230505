# Comparing `tmp/pathmatcher-1.8.0b2.tar.gz` & `tmp/pathmatcher-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathmatcher-1.8.0b2.tar", last modified: Thu Apr 27 22:06:41 2023, max compression
+gzip compressed data, was "pathmatcher-1.8.1.tar", last modified: Fri May  5 19:09:16 2023, max compression
```

## Comparing `pathmatcher-1.8.0b2.tar` & `pathmatcher-1.8.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/
--rw-rw-rw-   0        0        0     1093 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/LICENSE
--rw-rw-rw-   0        0        0       69 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0    32620 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/PKG-INFO
--rw-rw-rw-   0        0        0    29868 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/
--rw-rw-rw-   0        0        0      168 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/_version.py
--rw-rw-rw-   0        0        0     1955 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/expandhelper.m
--rw-rw-rw-   0        0        0     8063 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/functionalcoreg.m
-drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/
--rw-rw-rw-   0        0        0     2123 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/README.rst
--rw-rw-rw-   0        0        0      331 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/__init__.py
--rw-rw-rw-   0        0        0    61177 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/awmstools.py
--rw-rw-rw-   0        0        0     5267 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabcom.py
--rw-rw-rw-   0        0        0    18096 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabpipe.py
--rw-rw-rw-   0        0        0     1069 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabraw.py
--rw-rw-rw-   0        0        0    33031 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabwrap.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/pathlib2/
--rw-rw-rw-   0        0        0    54694 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/pathlib2/__init__.py
--rw-rw-rw-   0        0        0    43942 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/pathmatcher.py
--rw-rw-rw-   0        0        0     3066 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/realignhelper.m
--rw-rw-rw-   0        0        0      928 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/regex_files.m
--rw-rw-rw-   0        0        0    62358 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/reorientation_registration_helper.py
--rw-rw-rw-   0        0        0      227 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/reorienthelper.m
--rw-rw-rw-   0        0        0     3297 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/tee.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher.egg-info/
--rw-rw-rw-   0        0        0    32620 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9954 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/
+-rw-rw-rw-   0        0        0     1093 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    32439 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29842 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/pathmatcher/
+-rw-rw-rw-   0        0        0      168 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/_version.py
+-rw-rw-rw-   0        0        0     1955 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/expandhelper.m
+-rw-rw-rw-   0        0        0     8063 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/functionalcoreg.m
+drwxrwxrwx   0        0        0        0 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/pathmatcher/mlabwrap/
+-rw-rw-rw-   0        0        0     2123 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/README.rst
+-rw-rw-rw-   0        0        0      331 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/__init__.py
+-rw-rw-rw-   0        0        0    61177 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/awmstools.py
+-rw-rw-rw-   0        0        0     5267 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/matlabcom.py
+-rw-rw-rw-   0        0        0    18096 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/matlabpipe.py
+-rw-rw-rw-   0        0        0     1069 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/mlabraw.py
+-rw-rw-rw-   0        0        0    33031 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/mlabwrap/mlabwrap.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/pathmatcher/pathlib2/
+-rw-rw-rw-   0        0        0    54694 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/pathlib2/__init__.py
+-rw-rw-rw-   0        0        0    43942 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/pathmatcher.py
+-rw-rw-rw-   0        0        0     3066 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/realignhelper.m
+-rw-rw-rw-   0        0        0      928 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/regex_files.m
+-rw-rw-rw-   0        0        0    62358 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/reorientation_registration_helper.py
+-rw-rw-rw-   0        0        0      227 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/reorienthelper.m
+-rw-rw-rw-   0        0        0     3297 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pathmatcher/tee.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/pathmatcher.egg-info/
+-rw-rw-rw-   0        0        0    32439 2023-05-05 19:09:16.000000 pathmatcher-1.8.1/pathmatcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2023-05-05 19:09:16.000000 pathmatcher-1.8.1/pathmatcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:09:16.000000 pathmatcher-1.8.1/pathmatcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2023-05-05 19:09:16.000000 pathmatcher-1.8.1/pathmatcher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-05 19:09:16.000000 pathmatcher-1.8.1/pathmatcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 19:09:16.000000 pathmatcher-1.8.1/pathmatcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9819 2023-05-05 19:07:11.000000 pathmatcher-1.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:09:16.859052 pathmatcher-1.8.1/setup.cfg
```

### Comparing `pathmatcher-1.8.0b2/LICENSE` & `pathmatcher-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/PKG-INFO` & `pathmatcher-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathmatcher
-Version: 1.8.0b2
+Version: 1.8.1
 Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
 Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/pathmatcher
 Project-URL: Documentation, https://github.com/lrq3000/pathmatcher/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/pathmatcher
@@ -30,17 +30,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENSE
 
 # Pathmatcher: Manipulate file paths trees like simple text using powerful regular expressions!
@@ -51,42 +48,42 @@
 
 Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
 
 If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
 
 If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
 
-This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled reorientation_registration_helper.py submodule, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
+This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled `reorientation_registration_helper` command, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
 
 This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. As a Python module, it can not only match input paths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
 
 Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
 
 If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
 For Python 3.7+:
 
 ```
-pip install --upgrade pathmatcher
+pip install --upgrade pathmatcher --use-pep517
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
 For the latest development release, use:
 
 ```
-pip install --upgrade pathmatcher --pre
+pip install --upgrade pathmatcher --pre --use-pep517
 ```
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 ```
-pip install --upgrade git+https://github.com/lrq3000/pathmatcher
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher --pre --use-pep517
 ```
 
 For Python 2.7 to 3.6, the last compatible version is v1.7.6:
 
 ```
 pip install --upgrade pathmatcher==1.7.6
 ```
@@ -298,58 +295,58 @@
 
 * **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
 * scandir (for faster file walking and simulation report)
 * Gooey (for gui)
 
 ## Tutorial
 
-Here is a short introduction in the usage of `pathmatcher.py`.
+Here is a short introduction in the usage of `pathmatcher`.
 
-The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
+The most important trick to use `pathmatcher` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
 
 Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
 
 To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
 
 Now, in the commandline, execute the two following commands:
 
 ```python
-python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+pathmatcher -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
 
-python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+pathmatcher -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
 ```
 
 Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
 
 Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
 
-After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
+After executing both of these commands, `pathmatcher` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
 
 This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
 
 ```python
-python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+pathmatcher -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
 
-python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
+pathmatcher -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
 ```
 
 Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
 
 ```python
-python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
+pathmatcher -i "ABIDE/" -ri "mprage.nii.gz"
 ```
 
 This will generate the whole list of T1 and show them in a report.
 
 Of course, you can also use absolute paths for `--input` and `--output`.
 
 And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
 
 ```python
-python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+pathmatcher -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
 ```
 
 Result:
 
 ```
 == Regex Path Matcher started ==
 
@@ -365,27 +362,27 @@
 
 Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
 
 
 End of simulation. 1 files matched.
 ```
 
-Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
+Finally, `pathmatcher` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
 
 ```python
 from pathmatcher import main as pm
 
 # Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
 # You can use the commandline arguments, but the script will be called without bash but directly inside Python
 my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
 
 print(my_results)
 ```
 
-A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
+A concrete example of scripting of `pathmatcher` can be found inside the `reorientation_registration_helper` companion script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
 
 ### Similar projects
 
 A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
 
 ## Auxiliary tool: Reorientation and registration helper
```

### Comparing `pathmatcher-1.8.0b2/README.md` & `pathmatcher-1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,42 +6,42 @@
 
 Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
 
 If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
 
 If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
 
-This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled reorientation_registration_helper.py submodule, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
+This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled `reorientation_registration_helper` command, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
 
 This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. As a Python module, it can not only match input paths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
 
 Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
 
 If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
 For Python 3.7+:
 
 ```
-pip install --upgrade pathmatcher
+pip install --upgrade pathmatcher --use-pep517
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
 For the latest development release, use:
 
 ```
-pip install --upgrade pathmatcher --pre
+pip install --upgrade pathmatcher --pre --use-pep517
 ```
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 ```
-pip install --upgrade git+https://github.com/lrq3000/pathmatcher
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher --pre --use-pep517
 ```
 
 For Python 2.7 to 3.6, the last compatible version is v1.7.6:
 
 ```
 pip install --upgrade pathmatcher==1.7.6
 ```
@@ -253,58 +253,58 @@
 
 * **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
 * scandir (for faster file walking and simulation report)
 * Gooey (for gui)
 
 ## Tutorial
 
-Here is a short introduction in the usage of `pathmatcher.py`.
+Here is a short introduction in the usage of `pathmatcher`.
 
-The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
+The most important trick to use `pathmatcher` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
 
 Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
 
 To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
 
 Now, in the commandline, execute the two following commands:
 
 ```python
-python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+pathmatcher -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
 
-python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+pathmatcher -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
 ```
 
 Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
 
 Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
 
-After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
+After executing both of these commands, `pathmatcher` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
 
 This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
 
 ```python
-python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+pathmatcher -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
 
-python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
+pathmatcher -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
 ```
 
 Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
 
 ```python
-python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
+pathmatcher -i "ABIDE/" -ri "mprage.nii.gz"
 ```
 
 This will generate the whole list of T1 and show them in a report.
 
 Of course, you can also use absolute paths for `--input` and `--output`.
 
 And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
 
 ```python
-python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+pathmatcher -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
 ```
 
 Result:
 
 ```
 == Regex Path Matcher started ==
 
@@ -320,27 +320,27 @@
 
 Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
 
 
 End of simulation. 1 files matched.
 ```
 
-Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
+Finally, `pathmatcher` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
 
 ```python
 from pathmatcher import main as pm
 
 # Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
 # You can use the commandline arguments, but the script will be called without bash but directly inside Python
 my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
 
 print(my_results)
 ```
 
-A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
+A concrete example of scripting of `pathmatcher` can be found inside the `reorientation_registration_helper` companion script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
 
 ### Similar projects
 
 A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
 
 ## Auxiliary tool: Reorientation and registration helper
```

### Comparing `pathmatcher-1.8.0b2/pathmatcher/expandhelper.m` & `pathmatcher-1.8.1/pathmatcher/expandhelper.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/functionalcoreg.m` & `pathmatcher-1.8.1/pathmatcher/functionalcoreg.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/README.rst` & `pathmatcher-1.8.1/pathmatcher/mlabwrap/README.rst`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/awmstools.py` & `pathmatcher-1.8.1/pathmatcher/mlabwrap/awmstools.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabcom.py` & `pathmatcher-1.8.1/pathmatcher/mlabwrap/matlabcom.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabpipe.py` & `pathmatcher-1.8.1/pathmatcher/mlabwrap/matlabpipe.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabraw.py` & `pathmatcher-1.8.1/pathmatcher/mlabwrap/mlabraw.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabwrap.py` & `pathmatcher-1.8.1/pathmatcher/mlabwrap/mlabwrap.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/pathlib2/__init__.py` & `pathmatcher-1.8.1/pathmatcher/pathlib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/pathmatcher.py` & `pathmatcher-1.8.1/pathmatcher/pathmatcher.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/realignhelper.m` & `pathmatcher-1.8.1/pathmatcher/realignhelper.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/regex_files.m` & `pathmatcher-1.8.1/pathmatcher/regex_files.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/reorientation_registration_helper.py` & `pathmatcher-1.8.1/pathmatcher/reorientation_registration_helper.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher/tee.py` & `pathmatcher-1.8.1/pathmatcher/tee.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pathmatcher.egg-info/PKG-INFO` & `pathmatcher-1.8.1/pathmatcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathmatcher
-Version: 1.8.0b2
+Version: 1.8.1
 Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
 Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/pathmatcher
 Project-URL: Documentation, https://github.com/lrq3000/pathmatcher/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/pathmatcher
@@ -30,17 +30,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENSE
 
 # Pathmatcher: Manipulate file paths trees like simple text using powerful regular expressions!
@@ -51,42 +48,42 @@
 
 Patchmatcher is a files and folders hierarchy management tool in python, with a regular expression matcher on _paths_ (instead of just filenames). Can display a simulation report and automatically detect conflicts (already existing files, collisions of multiple files copied to the same output filename because of regexp, etc.). Can also be used as a Python module that returns the list of matched files and the transformations.
 
 If you often run experiments, you use scripts and applications, with some that you didn't design yourself. It might then happen that these apps/scripts expect a specific directory layout to work. Usually, you reorganize your files manually. Not only is this time consuming, this is also very error prone (eg, copying the wrong files to the wrong id).
 
 If you happen to know this situation, this tool might help you: just specify a regular expression matching the files you need, enter an output regular expression (that can reuse parts of the input files, for example your subjects ids, using regexp groups and recall), and then launch the program.
 
-This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled reorientation_registration_helper.py submodule, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
+This module works for any file management purpose, although it was primarily created to work for neuroimaging preprocessing tasks, such as reorganizing very fast any dataset into a BIDS compliant format. It can also be combined with the bundled `reorientation_registration_helper` command, showcasing how this module can be combined with MATLAB and SPM to semi-automate the manual anatomical reorientation of brain images to the AC-PC plane.
 
 This application can also be used as a Python module, so that you can include it in a pipeline to (semi-)automate repetitive stuff, like selecting the appropriate files to open in your favorite tool like SPM. As a Python module, it can not only match input paths, but also group them dynamically in a tree-like structure (a recursive dict) depending on the named regexp groups. This is a very useful and powerful too to quickly match multi-modal data and group them together (eg, structural and functional images) together, per subject and per study, in a single command. See `reorient_registration_helper.py` for an example use.
 
 Runs on Python 3 (Python 3.7 and 3.8 tested), and a previous version worked for Python 2.7.15 although compatibility isn't guaranteed anymore since Python 2 support is now deprecated.
 
 If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
 For Python 3.7+:
 
 ```
-pip install --upgrade pathmatcher
+pip install --upgrade pathmatcher --use-pep517
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
 For the latest development release, use:
 
 ```
-pip install --upgrade pathmatcher --pre
+pip install --upgrade pathmatcher --pre --use-pep517
 ```
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 ```
-pip install --upgrade git+https://github.com/lrq3000/pathmatcher
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher --pre --use-pep517
 ```
 
 For Python 2.7 to 3.6, the last compatible version is v1.7.6:
 
 ```
 pip install --upgrade pathmatcher==1.7.6
 ```
@@ -298,58 +295,58 @@
 
 * **[tqdm](https://github.com/tqdm/tqdm/)** (for progress bar, **highly recommended**)
 * scandir (for faster file walking and simulation report)
 * Gooey (for gui)
 
 ## Tutorial
 
-Here is a short introduction in the usage of `pathmatcher.py`.
+Here is a short introduction in the usage of `pathmatcher`.
 
-The most important trick to use `pathmatcher.py` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
+The most important trick to use `pathmatcher` efficiently that you should remember is this one: **try to break operations over multiple commands**. Indeed, it's simpler to match anatomical first, then functional, then dwi, etc... Rather than trying to match and reorder them all in only one command (which is possible but hard, for exactly the same result!).
 
 Let's take a concrete example: we are going to reorganize the NIfTI files from the [ABIDE I dataset](http://fcon_1000.projects.nitrc.org/indi/abide/) to the [BIDS scheme](http://bids.neuroimaging.io/).
 
 To do that, first create a directory anywhere you want (we will call this directory the "root directory", and unzip inside all ABIDE I dataset in one folder "ABIDE" (just "unzip here" the ABIDE I archives and this will create the `ABIDE` folder with the expected scheme). Then, inside the root directory, create another folder `ABIDE-BIDS` just beside the `ABIDE` folder. Now, open a terminal/console, and `cd` to the root directory, where there are now two subdirectories: "ABIDE" with ABIDE1 data, and `ABIDE-BIDS` that is empty.
 
 Now, in the commandline, execute the two following commands:
 
 ```python
-python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+pathmatcher -ri "Caltech_([0-9]+)/\dir/scans/anat/resources/NIfTI/files/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
 
-python pathmatcher.py -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
+pathmatcher -ri "Caltech_([0-9]+)/\dir/scans/rest/resources/NIfTI/files/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz" -i ABIDE/ -o ABIDE-BIDS/ -c
 ```
 
 Where `-i = --input` (base input directory), `-o = --output` (base output directory where files will get copied/moved), `-ri = --regex_input` (regular expression to match input files), `-ro = --regex_output` (regular expression to copy/move input files to output folder), `-c = --copy` (to enable copy mode, can also --symlink, --move, --delete). Note that you can type `--help` to get an extensive documentation of the arguments along with advices.
 
 Note also that `\dir` is an alias for `[^/\]*`, which allows to reliably match any directory in the path. Note also that `--regex_input` (`-ri`) and `--regex_output` (`-ro`) are matching paths relative to the `--input` and `--output` folders, thus nothing above `--input` and `--output` exist for pathmatcher. This was done so for two reasons: to more easily make your regexp (because you don't have to care about any parent folder from your `--input` or `--output`), and because of safety (to avoid `--delete` on your disk root! You are guaranteed that patchmatcher only works on subdirs).
 
-After executing both of these commands, `pathmatcher.py` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
+After executing both of these commands, `pathmatcher` will generate a report detailing all file operations it will do, and eventually warn you about conflicts (files getting the same filename and thus collisionning in the output folder).
 
 This works alright, converting the `ABIDE I` dataset scheme to `BIDS`, but this can be made simpler. Pathmatcher was made to allow for loose matching, so basically the idea is that you should try to match only the things that are necessary for you (either for recapture to use in the output like subject's id, or just to disambiguate like the folder name). Here are two simplified commands doing the same thing as above:
 
 ```python
-python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+pathmatcher -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
 
-python pathmatcher.py -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
+pathmatcher -c -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/rest.nii.gz" -ro "sub-\1/func/sub-\1_task-rest_bold.nii.gz"
 ```
 
 Also partial matching is supported, so if you just want to get the list of all T1, you can do the following:
 
 ```python
-python pathmatcher.py -i "ABIDE/" -ri "mprage.nii.gz"
+pathmatcher -i "ABIDE/" -ri "mprage.nii.gz"
 ```
 
 This will generate the whole list of T1 and show them in a report.
 
 Of course, you can also use absolute paths for `--input` and `--output`.
 
 And a last trick to help you when you design the regular expressions: use the `--test` argument to see if it matches at least one file, and what operation will be done:
 
 ```python
-python pathmatcher.py -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
+pathmatcher -c --test -i "ABIDE/" -o "ABIDE-BIDS/" -ri "Caltech_([0-9]+)/.+/mprage.nii.gz" -ro "sub-\1/anat/sub-\1_T1w.nii.gz"
 ```
 
 Result:
 
 ```
 == Regex Path Matcher started ==
 
@@ -365,27 +362,27 @@
 
 Match: Caltech_51456/Caltech_51456/scans/anat/resources/NIfTI/files/mprage.nii.gz --> sub-51456/anat/sub-51456_T1w.nii.gz
 
 
 End of simulation. 1 files matched.
 ```
 
-Finally, `pathmatcher.py` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
+Finally, `pathmatcher` can be used as an integral part of your own scripts, by either using it on commandline with the `--yes` argument to skip the report, or from your own python script by using the following:
 
 ```python
 from pathmatcher import main as pm
 
 # Match all T1 from ABIDE I, don't forget the r'' to avoid conflicts with / character
 # You can use the commandline arguments, but the script will be called without bash but directly inside Python
 my_results = pm(r'-i "ABIDE/" -ri "mprage.nii.gz"', return_report=True)  # use return_report=True to get the matches returned to your my_results variable
 
 print(my_results)
 ```
 
-A concrete example of scripting of `pathmatcher.py` can be found inside the `reorientation_registration_helper.py` script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
+A concrete example of scripting of `pathmatcher` can be found inside the `reorientation_registration_helper` companion script, which streamlines the manual preprocessing of fMRI data (reorientation, coregistration, quality and motion assessment, generation of composite motion metrics such as framewise median absolute deviation, etc).
 
 ### Similar projects
 
 A similar project, and potentially more powerful, is [fselect](https://github.com/jhspetersson/fselect), which allows to use SQL-like queries on files. In MATLAB, similar functions are available in [dirPlus](https://github.com/kpeaton/dirPlus).
 
 ## Auxiliary tool: Reorientation and registration helper
```

### Comparing `pathmatcher-1.8.0b2/pathmatcher.egg-info/SOURCES.txt` & `pathmatcher-1.8.1/pathmatcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0b2/pyproject.toml` & `pathmatcher-1.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,14 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Programming Language :: Python :: Implementation :: PyPy',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Utilities',
-    'Intended Audience :: Developers',
-    'Intended Audience :: End Users/Desktop',
-    'Intended Audience :: System Administrators',
 ]
 dependencies = [
     #"typing-extensions; python_version<'3.8'",
     #"importlib_metadata;python_version<'3.8'",
     "chardet>=3.0.4",
     "tqdm>=4.46.0",
     "scandir>=1.10.0",
```

