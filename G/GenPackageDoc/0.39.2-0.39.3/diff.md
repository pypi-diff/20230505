# Comparing `tmp/GenPackageDoc-0.39.2.tar.gz` & `tmp/GenPackageDoc-0.39.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenPackageDoc-0.39.2.tar", last modified: Wed Apr 26 12:05:48 2023, max compression
+gzip compressed data, was "GenPackageDoc-0.39.3.tar", last modified: Fri May  5 14:02:42 2023, max compression
```

## Comparing `GenPackageDoc-0.39.2.tar` & `GenPackageDoc-0.39.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/GenPackageDoc/
--rw-r--r--   0 runner    (1001) docker     (123)    40053 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CDocBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    25033 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CPackageDocConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CPatterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CSourceParser.py
--rw-r--r--   0 runner    (1001) docker     (123)   283914 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/GenPackageDoc.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/GenPackageDoc/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/admonitions.sty
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/common.sty
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/pandoc.sty
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/preamble.tex
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/robotframeworkaio.sty
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.478193 GenPackageDoc-0.39.3/GenPackageDoc/
+-rw-r--r--   0 runner    (1001) docker     (123)    40053 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CDocBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25033 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CPackageDocConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CPatterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/CSourceParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   277945 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc/GenPackageDoc.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/GenPackageDoc/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/admonitions.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/common.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/pandoc.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/preamble.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/styles/robotframeworkaio.sty
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/GenPackageDoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 14:02:42.000000 GenPackageDoc-0.39.3/GenPackageDoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:02:42.482193 GenPackageDoc-0.39.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-05 14:00:04.000000 GenPackageDoc-0.39.3/setup.py
```

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/CDocBuilder.py` & `GenPackageDoc-0.39.3/GenPackageDoc/CDocBuilder.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/CInterface.py` & `GenPackageDoc-0.39.3/GenPackageDoc/CInterface.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/CPackageDocConfig.py` & `GenPackageDoc-0.39.3/GenPackageDoc/CPackageDocConfig.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/CPatterns.py` & `GenPackageDoc-0.39.3/GenPackageDoc/CPatterns.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/CSourceParser.py` & `GenPackageDoc-0.39.3/GenPackageDoc/CSourceParser.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/GenPackageDoc.pdf` & `GenPackageDoc-0.39.3/GenPackageDoc/GenPackageDoc.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 GenPackageDoc
-v. 0.39.0
+v. 0.39.3
 Holger Queckenstedt
-06.01.2023
+05.05.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -111,41 +111,48 @@
 4.1.1
 
 11
 
 Method: GetLaTeXStyles . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5 CPackageDocConfig.py
+
+12
+
 5.1
 
+Function: printerror . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
 12
 
+5.2
+
 Class: CPackageDocConfig . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 12
 
-5.1.1
+5.2.1
 
 Method: PrintConfig . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 12
 
-5.1.2
+5.2.2
 
 Method: PrintConfigKeys . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 12
 
-5.1.3
+5.2.3
 
 Method: Get . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 12
 
-5.1.4
+5.2.4
 
 Method: GetConfig
 
 12
 
 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
@@ -179,34 +186,35 @@
 6.1.4
 
 Method: GetAutodefinedHeader . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 14
 
 7 CSourceParser.py
-7.1
 
 15
 
-Class: CSourceParser . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
 A
 
-15
-
 CONTENTS
 
-7.1.1
+7.1
 
 CONTENTS
 
-Method: ParseSourceFile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Class: CSourceParser . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 15
 
+7.1.1
+
+15
+
+Method: ParseSourceFile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
 8 Appendix
 
 16
 
 9 History
 
 17
@@ -253,29 +261,34 @@
 
 Description
 2.1
 
 Repository content
 
 What is the content of the repository python-genpackagedoc?
-• Folder GenPackageDoc
+ Folder GenPackageDoc
+
 Contains the package code.
 This folder is specific for the package.
-• Folder config
+ Folder config
+
 Contains the repository configuration (e.g. the name of the package, the name of the repository, the author,
 and more ...).
 This folder is specific for the repository.
-• Folder additions
+ Folder additions
+
 Contains additionally needed sources like setup related class definitions and sources, that are imported from
 other repositories - to make this repository stand alone
-• Folder packagedoc
+ Folder packagedoc
+
 Contains all package documentation related files, e.g. the GenPackageDoc configuration, additional input
 files and the generated documentation itself.
 This folder is specific for the documentation.
-• Repository root folder
+ Repository root folder
+
 – genpackagedoc.py
 Python script to start the documentation build
 – setup.py
 Python script to install the package sources. This includes the execution of genpackagedoc.py. Therefore building the documentation is part of the installation process.
 – dump repository config.py
 Little helper to dump the repository configuration to console
 – readme.rst2md.py
@@ -289,49 +302,55 @@
 2.2
 
 2.2. DOCUMENTATION BUILD PROCESS
 
 Documentation build process
 
 How do the files and folders listed above, belong together? What is the way, the information flows when the documentation is generated?
-• The process starts with the execution of genpackagedoc.py within the repository root folder.
+ The process starts with the execution of genpackagedoc.py within the repository root folder.
+
 genpackagedoc.py can be used stand alone - but this script is also called by setup.py. The impact is that
 every installation includes an update of the documentation.
-• genpackagedoc.py creates a repository configuration object
+ genpackagedoc.py creates a repository configuration object
+
 config/CRepositoryConfig.py
-• The repository configuration object reads the static repository configuration values out of a separate json file
+ The repository configuration object reads the static repository configuration values out of a separate json file
+
 config/repository config.json
-• The repository configuration object adds dynamic values (like operating system specific settings and paths)
+ The repository configuration object adds dynamic values (like operating system specific settings and paths)
 to the repository configuration. Not all of them are required for the documentation build process, but the
 repository configuration also supports the setup process (setup.py).
+
 There is one certain setting in the repository configuration file
 config/repository config.json,
 that is essential for the documentation build process:
 "PACKAGEDOC" : "./packagedoc"
 This is the path to a folder, in which all further documentation related files are placed. In case of the path
 is relative, the reference is the position of genpackagedoc.py. It is required that within this folder the
 configuration file for the documentation build process
 packagedoc config.json
 can be found. The name of this json file is fix!
-• The configuration file packagedoc config.json contains settings like
+ The configuration file packagedoc config.json contains settings like
+
 – Paths to Python packages to be documented
 – Paths and names of additional RST files
 – Path and name of output folder (LaTeX files and output PDF file)
 – User defined parameter (that can be defined here as global runtime variables and can be used in any RST
 code)
 – Basic settings related to the output PDF file (like document name, name of author, ...)
 – Path to LaTeX compiler
 (a LaTeX distribution is not part of GenPackageDoc)
 Be aware of that the within packagedoc config.json specified output folder
 "OUTPUT" : "./build"
 will be deleted at the beginning of the documentation build process! Make sure that you do not have any files
 inside this folder opened when you start the process. In case of the path is relative, the reference is the position
 of genpackagedoc.py. The complete path is created recursively.
 Further details are explained within the json file itself.
-• genpackagedoc.py also creates an own configuration object
+ genpackagedoc.py also creates an own configuration object
+
 GenPackageDoc/CPackageDocConfig.py
 CPackageDocConfig.py takes over all repository configuration values, reads in the static GenPackageDoc
 configuration (packagedoc config.json) and adds dynamically computed values like the full absolute paths
 belonging to the documentation build process. Also all command line parameters are resolved and checked.
 The reference for all relative paths is the position of genpackagedoc.py (that is the repository root folder).
 3
 
@@ -388,28 +407,32 @@
 PDF document structure
 
 How is the resulting PDF document structured? What causes an entry within the table of content of the PDF document?
 In the following we use terms taken over from the LaTeX world: chapter, section and subsection.
 A chapter is the top level within the PDF document; a section is the level below chapter, a subsection is the level
 below section.
 The following assignments happen during the generation of a PDF document:
-• The content of every additionally included separate RST file is a chapter.
+ The content of every additionally included separate RST file is a chapter.
+
 – In case of you want to add another chapter to your documentation, you have to include another RST file.
 – The headline of the chapter is the name of the RST file (automatically).
 Therefore the heading within an RST file has to start at section level!
-• The content of every included Python module is also a chapter.
+ The content of every included Python module is also a chapter.
+
 – The headline of the chapter is the name of the Python module (automatically).
 This means also that within the PDF document structure every Python module is at the same level as
 additionally included RST files.
-• Within additionally included separate RST files sections and subsections can be defined by the following RST
+ Within additionally included separate RST files sections and subsections can be defined by the following RST
 syntax elements for headings:
+
 – A line underlined with ”=” characters is a section
 – A line underlined with ”-” characters is a subsection
-• Within the docstrings of Python modules the headings are added automatically (for functions, classes and
+ Within the docstrings of Python modules the headings are added automatically (for functions, classes and
 methods)
+
 – Classes and functions are listed at section level (both classes and functions are assumed to be at the same
 level).
 – Class methods are listed at subesction level.
 Further nestings of headings are not supported (because we do not want to overload the table of content).
 
 5
 
@@ -533,45 +556,49 @@
 2.7.1
 
 Common rules
 
 2.7. SYNTAX ASPECTS
 
 Important to know about the syntax of Python and RST is:
-• In both Python and RST the indentation of text is part of the syntax!
-• The indentation of the triple quotes indicating the beginning and the end of a docstring has to follow the Python
+ In both Python and RST the indentation of text is part of the syntax!
+ The indentation of the triple quotes indicating the beginning and the end of a docstring has to follow the Python
 syntax rules.
-• The indentation of the content of the docstring (= the interface description in RST format) has to follow the
+ The indentation of the content of the docstring (= the interface description in RST format) has to follow the
 RST syntax rules. To avoid a needless indentation of the text within the resulting PDF document and to avoid
 further unwanted side effects caused by improper indentations, it is strongly required to start at least the first
 line of a docstring text within the first column! And this first line is the reference for the indentation of further
 lines of the current docstring. The indentation of these further lines depends on the RST syntax element that
 is used here.
-• In RST also blank lines are part of the syntax!
+ In RST also blank lines are part of the syntax!
+
 Why is a proper indentation of the docstrings so much important?
 The contents of all doctrings of a Python module will be merged to one single RST document (internally by GenPackageDoc). In this single RST document we do not have separated docstring lines any more. We have one text!
 And we have a relationship between previous lines and following lines in this text. The indentation of these previous
 and following lines must fit together – accordingly to the RST syntax rules. Otherwise we either get syntax issues
 during computation or we get text with a layout that does not fit to our expectation.
 Please be attentive while typing your documentation in RST format!
 
 2.7.2
 
 Syntax extensions
 
 GenPackageDoc extends the RST syntax by the following topics:
-• newline
+ newline
+
 A newline (line break) is realized by a slash (’/’) at the end of a line containing any other RST text (this means:
 the slash must not be the only character in line).
 Internally this slash is mapped to the LaTeX command \newline.
-• vspace
+ vspace
+
 An additional vertical space (size: the height of the ’x’ character - depending on the current type and size of
 font) is realized by a single slash (’/’). This slash must be the only character in line!
 Internally this slash is mapped to the LaTeX command \vspace{1ex}.
-• newpage
+ newpage
+
 A newpage (page break) is realized by a double slash (’//’). These two slashes must be the only characters in
 line!
 Internally this double slash is mapped to the LaTeX command \newpage.
 These syntax extensions can currently be used in separate RST files only and are not available within docstrings of
 Python modules.
 
 9
@@ -597,18 +624,20 @@
 3.1.1
 
 Method: Build
 
 Arguments:
 (no arguments)
 Returns:
-• bSuccess
+ bSuccess
+
 / Type: bool /
 Indicates if the computation of the method sMethod was successful or not.
-• sResult
+ sResult
+
 / Type: str /
 The result of the computation of the method sMethod.
 
 10
 
 CHAPTER 4. CINTERFACE.PY
 
@@ -628,22 +657,25 @@
 4.1.1
 
 Method: GetLaTeXStyles
 
 The LaTeX stylesheets are part of the installation of GenPackageDoc. In case of anyone else than GenPackageDoc
 needs these stylesheets, this method can be used to copy them to any other folder.
 Arguments:
-• sDestination
+ sDestination
+
 / Condition: required / Type: str /
 Path and name of a folder in which the styles folder from GenPackageDoc will be copied.
 Returns:
-• bSuccess
+ bSuccess
+
 / Type: bool /
 Indicates if the computation of the method sMethod was successful or not.
-• sResult
+ sResult
+
 / Type: str /
 The result of the computation of the method sMethod.
 
 11
 
 CHAPTER 5. CPACKAGEDOCCONFIG.PY
 
@@ -651,38 +683,42 @@
 
 CPackageDocConfig.py
 Python module containing the configuration for GenPackageDoc. This includes the repository configurantion and
 command line values.
 
 5.1
 
+Function: printerror
+
+5.2
+
 Class: CPackageDocConfig
 
 Imported by:
 from GenPackageDoc.CPackageDocConfig import CPackageDocConfig
 
-5.1.1
+5.2.1
 
 Method: PrintConfig
 
 Prints all cofiguration values to console.
 
-5.1.2
+5.2.2
 
 Method: PrintConfigKeys
 
 Prints all cofiguration key names to console.
 
-5.1.3
+5.2.3
 
 Method: Get
 
 Returns the configuration value belonging to a key name.
 
-5.1.4
+5.2.4
 
 Method: GetConfig
 
 Returns the complete configuration dictionary.
 
 12
 
@@ -705,28 +741,33 @@
 
 6.1.1
 
 Method: GetHeader
 
 Defines the header of the main tex file.
 Arguments:
-• sTitle
+ sTitle
+
 / Condition: required / Type: str /
 The title of the output document (name of the described package)
-• sVersion
+ sVersion
+
 / Condition: required / Type: str /
 The version of the output document (version of the described package)
-• sAuthor
+ sAuthor
+
 / Condition: required / Type: str /
 The author of the output document (author of the described package)
-• sDate
+ sDate
+
 / Condition: required / Type: str /
 The date of the output document (date of the described package)
 Returns:
-• sHeader
+ sHeader
+
 / Type: str /
 LaTeX code containing the header of main tex file.
 
 13
 
 CHAPTER 6. CPATTERNS.PY
 
@@ -736,50 +777,56 @@
 
 Method: GetChapter
 
 Defines single chapter of the main tex file.
 A single chapter is equivalent to an additionally imported text file in rst format or equivalent to a single Python
 module within a Python package.
 Arguments:
-• sHeadline
+ sHeadline
+
 / Condition: required / Type: str /
 The chapter headline (that is either the name of an additional rst file or the name of a Python module).
-• sLabel
+ sLabel
+
 / Condition: required / Type: str /
 The chapter label (to enable linking to this chapter)
-• sDocumentName
+ sDocumentName
+
 / Condition: required / Type: str /
 The name of a single tex file containing the chapter content. This file is imported in the main text file after the
 chapter headline that is set by sHeadline.
 Returns:
-• sHeader
+ sHeader
+
 / Type: str /
 LaTeX code containing the headline and the input of a single tex file.
 
 6.1.3
 
 Method: GetFooter
 
 Defines the footer of the main tex file.
 Arguments:
 (no arguments)
 Returns:
-• sFooter
+ sFooter
+
 / Type: str /
 LaTeX code containing the footer of the main tex file.
 
 6.1.4
 
 Method: GetAutodefinedHeader
 
 Defines the header of the autodefined LaTeX sty file.
 Arguments:
 (no arguments)
 Returns:
-• sAutodefinedHeader
+ sAutodefinedHeader
+
 / Type: str /
 LaTeX code containing the header of the autodefined LaTeX sty file.
 
 14
 
 CHAPTER 7. CSOURCEPARSER.PY
 
@@ -799,32 +846,38 @@
 
 7.1.1
 
 Method: ParseSourceFile
 
 The method ParseSourceFile parses the content of a Python module.
 Arguments:
-• sFile
+ sFile
+
 / Condition: required / Type: str /
 Path and name of a single Python module.
-• bIncludePrivate (currently not active, is False)
+ bIncludePrivate (currently not active, is False)
+
 / Condition: optional / Type: bool / Default: False /
 If False: private methods are skipped, otherwise they are included in documentation.
-• bIncludeUndocumented
+ bIncludeUndocumented
+
 / Condition: optional / Type: bool / Default: True /
 If True: also classes and methods without docstring are listed in the documentation (together with a hint that
 information is not available), otherwise they are skipped.
 Returns:
-• dictContent
+ dictContent
+
 / Type: dict /
 A dictionary containing all the information parsed out of sFile.
-• bSuccess
+ bSuccess
+
 / Type: bool /
 Indicates if the computation of the method sMethod was successful or not.
-• sResult
+ sResult
+
 / Type: str /
 The result of the computation of the method sMethod.
 
 15
 
 CHAPTER 8. APPENDIX
 
@@ -839,19 +892,19 @@
 
 Name
 
 GenPackageDoc
 
 Version
 
-0.39.0
+0.39.3
 
 Date
 
-06.01.2023
+05.05.2023
 
 Description
 
 Documentation builder for Python packages
 
 Package URL
 
@@ -1134,13 +1187,13 @@
 
 06.01.2023
 
 Added masking of underlines in case of the content of \repo or \pkg contain
 underlines (masking required by LaTeX).
 
 GenPackageDoc.pdf
-Created at 06.01.2023 - 15:11:02
-by GenPackageDoc v. 0.39.0
+Created at 05.05.2023 - 14:02:38
+by GenPackageDoc v. 0.39.3
 
 19
```

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/__init__.py` & `GenPackageDoc-0.39.3/GenPackageDoc/__init__.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/styles/admonitions.sty` & `GenPackageDoc-0.39.3/GenPackageDoc/styles/admonitions.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/styles/common.sty` & `GenPackageDoc-0.39.3/GenPackageDoc/styles/common.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/styles/pandoc.sty` & `GenPackageDoc-0.39.3/GenPackageDoc/styles/pandoc.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/styles/preamble.tex` & `GenPackageDoc-0.39.3/GenPackageDoc/styles/preamble.tex`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/styles/robotframeworkaio.sty` & `GenPackageDoc-0.39.3/GenPackageDoc/styles/robotframeworkaio.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc/version.py` & `GenPackageDoc-0.39.3/GenPackageDoc/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of GenPackageDoc
 #
-VERSION      = "0.39.2"
-VERSION_DATE = "26.04.2023"
+VERSION      = "0.39.3"
+VERSION_DATE = "05.05.2023"
```

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc.egg-info/PKG-INFO` & `GenPackageDoc-0.39.3/GenPackageDoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.39.2
+Version: 0.39.3
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GenPackageDoc-0.39.2/GenPackageDoc.egg-info/SOURCES.txt` & `GenPackageDoc-0.39.3/GenPackageDoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/LICENSE` & `GenPackageDoc-0.39.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/PKG-INFO` & `GenPackageDoc-0.39.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.39.2
+Version: 0.39.3
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GenPackageDoc-0.39.2/README.rst` & `GenPackageDoc-0.39.3/README.rst`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.2/setup.py` & `GenPackageDoc-0.39.3/setup.py`

 * *Files identical despite different names*

