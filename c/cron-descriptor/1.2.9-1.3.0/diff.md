# Comparing `tmp/cron_descriptor-1.2.9.tar.gz` & `tmp/cron_descriptor-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cron_descriptor-1.2.9.tar", last modified: Fri Jul  7 17:01:28 2017, max compression
+gzip compressed data, was "cron_descriptor-1.3.0.tar", last modified: Fri May  5 12:10:03 2023, max compression
```

## Comparing `cron_descriptor-1.2.9.tar` & `cron_descriptor-1.3.0.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 sadam     (1000) sadam     (1000)        0 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     4561 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/README.md
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2099 2017-07-07 16:59:53.000000 cron_descriptor-1.2.9/setup.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1080 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/LICENSE
--rw-r--r--   0 sadam     (1000) sadam     (1000)       38 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/setup.cfg
-drwxr-xr-x   0 sadam     (1000) sadam     (1000)        0 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor.egg-info/
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1061 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor.egg-info/SOURCES.txt
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     6616 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor.egg-info/PKG-INFO
--rw-rw-r--   0 sadam     (1000) sadam     (1000)        1 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor.egg-info/dependency_links.txt
--rw-rw-r--   0 sadam     (1000) sadam     (1000)       22 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor.egg-info/top_level.txt
-drwxr-xr-x   0 sadam     (1000) sadam     (1000)        0 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor/
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1297 2017-07-07 17:00:05.000000 cron_descriptor-1.2.9/cron_descriptor/Options.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)      858 2017-07-07 17:00:05.000000 cron_descriptor-1.2.9/cron_descriptor/CasingTypeEnum.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1206 2017-07-07 17:00:06.000000 cron_descriptor-1.2.9/cron_descriptor/StringBuilder.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1304 2017-07-07 17:00:06.000000 cron_descriptor-1.2.9/cron_descriptor/Exception.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1483 2017-07-07 17:00:07.000000 cron_descriptor-1.2.9/cron_descriptor/GetText.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)    22443 2017-07-07 17:00:07.000000 cron_descriptor-1.2.9/cron_descriptor/ExpressionDescriptor.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     8000 2017-07-07 17:00:08.000000 cron_descriptor-1.2.9/cron_descriptor/ExpressionParser.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1171 2017-07-07 17:00:08.000000 cron_descriptor-1.2.9/cron_descriptor/__init__.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)      920 2017-07-07 17:00:08.000000 cron_descriptor-1.2.9/cron_descriptor/DescriptionTypeEnum.py
-drwxr-xr-x   0 sadam     (1000) sadam     (1000)        0 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/cron_descriptor/locale/
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2760 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/tr_TR.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2675 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/zh_CN.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2730 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/pt_PT.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     3177 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/sv_SE.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2841 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/fr_FR.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     3116 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/ru_RU.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2783 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/it_IT.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     3051 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/uk_UA.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2758 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/nb_NO.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2820 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/es_ES.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2701 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/de_DE.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2738 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/nl_NL.mo
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2949 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/cron_descriptor/locale/cs_CZ.mo
--rw-r--r--   0 sadam     (1000) sadam     (1000)     6616 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/PKG-INFO
--rw-rw-r--   0 sadam     (1000) sadam     (1000)       61 2017-01-25 19:59:54.000000 cron_descriptor-1.2.9/MANIFEST.in
-drwxr-xr-x   0 sadam     (1000) sadam     (1000)        0 2017-07-07 17:01:28.000000 cron_descriptor-1.2.9/tests/
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1825 2017-07-07 17:00:09.000000 cron_descriptor-1.2.9/tests/TestApi.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     2921 2017-07-07 17:00:09.000000 cron_descriptor-1.2.9/tests/TestExceptions.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1102 2017-07-07 17:00:10.000000 cron_descriptor-1.2.9/tests/TestLocale.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)    13766 2017-07-07 17:00:10.000000 cron_descriptor-1.2.9/tests/TestFormats.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1071 2017-07-07 17:00:10.000000 cron_descriptor-1.2.9/tests/TestCase.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1082 2017-07-07 17:00:11.000000 cron_descriptor-1.2.9/tests/__init__.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1825 2017-07-07 17:00:11.000000 cron_descriptor-1.2.9/tests/TestCasing.py
--rw-rw-r--   0 sadam     (1000) sadam     (1000)     1741 2017-07-07 17:00:12.000000 cron_descriptor-1.2.9/tests/TestImport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.682659 cron_descriptor-1.3.0/cron_descriptor/
+-rw-rw-rw-   0 root         (0) root         (0)     1276 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/CasingTypeEnum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/DescriptionTypeEnum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/Exception.py
+-rw-rw-rw-   0 root         (0) root         (0)    25057 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/ExpressionDescriptor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9459 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/ExpressionParser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/GetText.py
+-rw-rw-rw-   0 root         (0) root         (0)     1697 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/Options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/StringBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/cron_descriptor/locale/
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/cs_CZ.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/de_DE.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/en_US.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/es_ES.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3203 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/fa_IR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/fr_FR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/it_IT.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ja_JP.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ko_KR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/nb_NO.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/nl_NL.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/pt_PT.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ru_RU.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/sk_SK.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/sv_SE.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4681 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/ta_IN.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/tr_TR.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/uk_UA.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/cron_descriptor/locale/zh_CN.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/cron_descriptor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-05 12:10:03.000000 cron_descriptor-1.3.0/cron_descriptor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 12:10:03.686659 cron_descriptor-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-05-05 12:09:07.000000 cron_descriptor-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cron_descriptor-1.2.9/README.md` & `cron_descriptor-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,107 @@
 # Cron Descriptor
 
-Master: [![Master Build Status](https://api.travis-ci.org/Salamek/cron-descriptor.svg?branch=master)](https://travis-ci.org/Salamek/cron-descriptor) All: [![Build Status](https://api.travis-ci.org/Salamek/cron-descriptor.svg)](https://travis-ci.org/Salamek/cron-descriptor)
-[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=D8LQ4XTBLV3C4&lc=CZ&item_number=Salamekcron-descriptor&currency_code=EUR)
+[![Python tests](https://github.com/Salamek/cron-descriptor/actions/workflows/python-test.yml/badge.svg)](https://github.com/Salamek/cron-descriptor/actions/workflows/python-test.yml)
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/salamek)
 
 A Python library that converts cron expressions into human readable strings. Ported to Python from https://github.com/bradyholt/cron-expression-descriptor.
 
 **Author**: Adam Schubert (https://www.salamek.cz)  
 **Original Author & Credit**: Brady Holt (http://www.geekytidbits.com)  
 **License**: [MIT](http://opensource.org/licenses/MIT)
 
 ## Features         
  * Supports all cron expression special characters including * / , - ? L W, #
  * Supports 5, 6 (w/ seconds or year), or 7 (w/ seconds and year) part cron expressions
  * Provides casing options (Sentence, Title, Lower, etc.)
- * Localization with support for 14 languages
- * Supports Python 2.7 - 3.4
+ * Localization with support for 17 languages
+ * Supports Python 2.7 - 3.10
 
 ## Installation
 Using PIP
 ```bash
 pip install cron-descriptor
 ```
 
 ## Usage example
 
+### Simple
 ```python
-# Simple
 from cron_descriptor import get_description, ExpressionDescriptor
 
 print(get_description("* 2 3 * *"))
 
 #OR
 
 print(str(ExpressionDescriptor("* 2 3 * *")))
 ```
 
+### Advanced
 ```python
-# Advanced
 # Consult Options.py/CasingTypeEnum.py/DescriptionTypeEnum.py for more info
 from cron_descriptor import Options, CasingTypeEnum, DescriptionTypeEnum, ExpressionDescriptor
 
-descripter = ExpressionDescriptor("*/10 * * * *", throw_exception_on_parse_error = True, casing_type = CasingTypeEnum.Sentence, use_24hour_time_format = True)
+descriptor = ExpressionDescriptor(
+    expression = "*/10 * * * *",
+    casing_type = CasingTypeEnum.Sentence,
+    use_24hour_time_format = True
+)
+
 # GetDescription uses DescriptionTypeEnum.FULL by default:
-print(descripter.get_description())
-print("{}".format(descripter))
+print(descriptor.get_description())
+print("{}".format(descriptor))
 
-#or passing Options class as second argument:
+# Or passing Options class as second argument:
 
 options = Options()
-options.throw_exception_on_parse_error = True
 options.casing_type = CasingTypeEnum.Sentence
 options.use_24hour_time_format = True
-descripter = ExpressionDescriptor("*/10 * * * *", options)
-print(descripter.get_description(DescriptionTypeEnum.FULL))
-
+descriptor = ExpressionDescriptor("*/10 * * * *", options)
+print(descriptor.get_description(DescriptionTypeEnum.FULL))
 ```
 
 ## Languages Available
-  * English ([Brady Holt](https://github.com/bradyholt))
-  * Brazilian ([Renato Lima](https://github.com/natenho))
-  * Spanish ([Ivan Santos](https://github.com/ivansg))
-  * Norwegian ([Siarhei Khalipski](https://github.com/KhalipskiSiarhei))
-  * Turkish ([Mustafa SADEDİL](https://github.com/sadedil))
-  * Dutch ([TotalMace](https://github.com/TotalMace))
-  * Chinese Simplified ([Star Peng](https://github.com/starpeng))
-  * Russian ([LbISS](https://github.com/LbISS))
-  * French ([Arnaud TAMAILLON](https://github.com/Greybird))
-  * German ([Michael Schuler](https://github.com/mschuler))
-  * Ukrainian ([Taras](https://github.com/tbudurovych))
-  * Italian ([rinaldihno](https://github.com/rinaldihno))
-  * Czech ([Adam Schubert](https://github.com/salamek))
-  * Swedish ([Åke Engelbrektson](https://github.com/eson57))
+
+|Language| Locale Code | Contributor |
+|--------|-------------|-------------|
+|English |en|[Brady Holt](https://github.com/bradyholt)|
+|Brazilian |pt_PT|[Renato Lima](https://github.com/natenho)|
+|Chinese Simplified | zh_CN |[Star Peng](https://github.com/starpeng)|
+|Spanish |es_ES|[Ivan Santos](https://github.com/ivansg)|
+|Norwegian |nb_NO|[Siarhei Khalipski](https://github.com/KhalipskiSiarhei)|
+|Turkish |tr_TR|[Mustafa SADEDİL](https://github.com/sadedil)|
+|Dutch |nl_NL|[TotalMace](https://github.com/TotalMace)|
+|Russian |ru_RU|[LbISS](https://github.com/LbISS)|
+|French |fr_FR|[Arnaud TAMAILLON](https://github.com/Greybird)|
+|German |de_DE|[Michael Schuler](https://github.com/mschuler)|
+|Ukrainian |uk_UA|[Taras](https://github.com/tbudurovych)|
+|Italian |it_IT|[rinaldihno](https://github.com/rinaldihno)|
+|Czech |cs_CZ|[Adam Schubert](https://github.com/salamek)|
+|Swedish |sv_SE|[Åke Engelbrektson](https://github.com/eson57)|
+|Tamil |ta_IN|[Sankar Hari](https://github.com/sankarhari)|
+|Persian|fa_IR|[M. Yas. Davoodeh](https://github.com/Davoodeh)|
+|Korean|ko_KR|[KyuJoo Han](https://github.com/hanqyu)|
+|Japanese |ja_JP|[Tho Nguyen](https://github.com/tho-asterist)|
 
 <!-- SOON
 ## Demo
 
 
 
 ## Download
 
 -->
 
 ## Original Source
  - .NET - [https://github.com/bradyholt/cron-expression-descriptor](https://github.com/bradyholt/cron-expression-descriptor)
 
 ## Ports
- - Java - [https://github.com/RedHogs/cron-parser](https://github.com/RedHogs/cron-parser)
- - Ruby - [https://github.com/alpinweis/cronex](https://github.com/alpinweis/cronex)
+ - Java     - [https://github.com/RedHogs/cron-parser](https://github.com/RedHogs/cron-parser)
+ - Ruby     - [https://github.com/alpinweis/cronex](https://github.com/alpinweis/cronex)
+ - Golang   - [https://github.com/jsuar/go-cron-descriptor](https://github.com/jsuar/go-cron-descriptor)
 
 ## Running Unit Tests
 
 ```bash
 python setup.py test
 ```
 
@@ -113,15 +124,15 @@
 Generating *.mo file from *.po file. In root directory run command:
 ```bash
 msgfmt -o cron_descriptor/locale/YOUR_LOCALE_CODE.mo cron_descriptor/locale/YOUR_LOCALE_CODE.po
 ```
 
 ## Developing
 
-All suggescions and PR's are welcomed
+All suggestions and PR's are welcomed
 
 Just clone this repository and register pre-commit hook by running:
 
 ```bash
 ln -s ../../pre-commit.sh .git/hooks/pre-commit
 ```
```

### Comparing `cron_descriptor-1.2.9/LICENSE` & `cron_descriptor-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor.egg-info/PKG-INFO` & `cron_descriptor-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,115 @@
-Metadata-Version: 1.1
-Name: cron-descriptor
-Version: 1.2.9
+Metadata-Version: 2.1
+Name: cron_descriptor
+Version: 1.3.0
 Summary: A Python library that converts cron expressions into human readable strings.
 Home-page: https://github.com/Salamek/cron-descriptor
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: UNKNOWN
 Description: # Cron Descriptor
         
-        Master: [![Master Build Status](https://api.travis-ci.org/Salamek/cron-descriptor.svg?branch=master)](https://travis-ci.org/Salamek/cron-descriptor) All: [![Build Status](https://api.travis-ci.org/Salamek/cron-descriptor.svg)](https://travis-ci.org/Salamek/cron-descriptor)
-        [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=D8LQ4XTBLV3C4&lc=CZ&item_number=Salamekcron-descriptor&currency_code=EUR)
+        [![Python tests](https://github.com/Salamek/cron-descriptor/actions/workflows/python-test.yml/badge.svg)](https://github.com/Salamek/cron-descriptor/actions/workflows/python-test.yml)
+        [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/salamek)
         
         A Python library that converts cron expressions into human readable strings. Ported to Python from https://github.com/bradyholt/cron-expression-descriptor.
         
         **Author**: Adam Schubert (https://www.salamek.cz)  
         **Original Author & Credit**: Brady Holt (http://www.geekytidbits.com)  
         **License**: [MIT](http://opensource.org/licenses/MIT)
         
         ## Features         
          * Supports all cron expression special characters including * / , - ? L W, #
          * Supports 5, 6 (w/ seconds or year), or 7 (w/ seconds and year) part cron expressions
          * Provides casing options (Sentence, Title, Lower, etc.)
-         * Localization with support for 14 languages
-         * Supports Python 2.7 - 3.4
+         * Localization with support for 17 languages
+         * Supports Python 2.7 - 3.10
         
         ## Installation
         Using PIP
         ```bash
         pip install cron-descriptor
         ```
         
         ## Usage example
         
+        ### Simple
         ```python
-        # Simple
         from cron_descriptor import get_description, ExpressionDescriptor
         
         print(get_description("* 2 3 * *"))
         
         #OR
         
         print(str(ExpressionDescriptor("* 2 3 * *")))
         ```
         
+        ### Advanced
         ```python
-        # Advanced
         # Consult Options.py/CasingTypeEnum.py/DescriptionTypeEnum.py for more info
         from cron_descriptor import Options, CasingTypeEnum, DescriptionTypeEnum, ExpressionDescriptor
         
-        descripter = ExpressionDescriptor("*/10 * * * *", throw_exception_on_parse_error = True, casing_type = CasingTypeEnum.Sentence, use_24hour_time_format = True)
+        descriptor = ExpressionDescriptor(
+            expression = "*/10 * * * *",
+            casing_type = CasingTypeEnum.Sentence,
+            use_24hour_time_format = True
+        )
+        
         # GetDescription uses DescriptionTypeEnum.FULL by default:
-        print(descripter.get_description())
-        print("{}".format(descripter))
+        print(descriptor.get_description())
+        print("{}".format(descriptor))
         
-        #or passing Options class as second argument:
+        # Or passing Options class as second argument:
         
         options = Options()
-        options.throw_exception_on_parse_error = True
         options.casing_type = CasingTypeEnum.Sentence
         options.use_24hour_time_format = True
-        descripter = ExpressionDescriptor("*/10 * * * *", options)
-        print(descripter.get_description(DescriptionTypeEnum.FULL))
-        
+        descriptor = ExpressionDescriptor("*/10 * * * *", options)
+        print(descriptor.get_description(DescriptionTypeEnum.FULL))
         ```
         
         ## Languages Available
-          * English ([Brady Holt](https://github.com/bradyholt))
-          * Brazilian ([Renato Lima](https://github.com/natenho))
-          * Spanish ([Ivan Santos](https://github.com/ivansg))
-          * Norwegian ([Siarhei Khalipski](https://github.com/KhalipskiSiarhei))
-          * Turkish ([Mustafa SADEDİL](https://github.com/sadedil))
-          * Dutch ([TotalMace](https://github.com/TotalMace))
-          * Chinese Simplified ([Star Peng](https://github.com/starpeng))
-          * Russian ([LbISS](https://github.com/LbISS))
-          * French ([Arnaud TAMAILLON](https://github.com/Greybird))
-          * German ([Michael Schuler](https://github.com/mschuler))
-          * Ukrainian ([Taras](https://github.com/tbudurovych))
-          * Italian ([rinaldihno](https://github.com/rinaldihno))
-          * Czech ([Adam Schubert](https://github.com/salamek))
-          * Swedish ([Åke Engelbrektson](https://github.com/eson57))
+        
+        |Language| Locale Code | Contributor |
+        |--------|-------------|-------------|
+        |English |en|[Brady Holt](https://github.com/bradyholt)|
+        |Brazilian |pt_PT|[Renato Lima](https://github.com/natenho)|
+        |Chinese Simplified | zh_CN |[Star Peng](https://github.com/starpeng)|
+        |Spanish |es_ES|[Ivan Santos](https://github.com/ivansg)|
+        |Norwegian |nb_NO|[Siarhei Khalipski](https://github.com/KhalipskiSiarhei)|
+        |Turkish |tr_TR|[Mustafa SADEDİL](https://github.com/sadedil)|
+        |Dutch |nl_NL|[TotalMace](https://github.com/TotalMace)|
+        |Russian |ru_RU|[LbISS](https://github.com/LbISS)|
+        |French |fr_FR|[Arnaud TAMAILLON](https://github.com/Greybird)|
+        |German |de_DE|[Michael Schuler](https://github.com/mschuler)|
+        |Ukrainian |uk_UA|[Taras](https://github.com/tbudurovych)|
+        |Italian |it_IT|[rinaldihno](https://github.com/rinaldihno)|
+        |Czech |cs_CZ|[Adam Schubert](https://github.com/salamek)|
+        |Swedish |sv_SE|[Åke Engelbrektson](https://github.com/eson57)|
+        |Tamil |ta_IN|[Sankar Hari](https://github.com/sankarhari)|
+        |Persian|fa_IR|[M. Yas. Davoodeh](https://github.com/Davoodeh)|
+        |Korean|ko_KR|[KyuJoo Han](https://github.com/hanqyu)|
+        |Japanese |ja_JP|[Tho Nguyen](https://github.com/tho-asterist)|
         
         <!-- SOON
         ## Demo
         
         
         
         ## Download
         
         -->
         
         ## Original Source
          - .NET - [https://github.com/bradyholt/cron-expression-descriptor](https://github.com/bradyholt/cron-expression-descriptor)
         
         ## Ports
-         - Java - [https://github.com/RedHogs/cron-parser](https://github.com/RedHogs/cron-parser)
-         - Ruby - [https://github.com/alpinweis/cronex](https://github.com/alpinweis/cronex)
+         - Java     - [https://github.com/RedHogs/cron-parser](https://github.com/RedHogs/cron-parser)
+         - Ruby     - [https://github.com/alpinweis/cronex](https://github.com/alpinweis/cronex)
+         - Golang   - [https://github.com/jsuar/go-cron-descriptor](https://github.com/jsuar/go-cron-descriptor)
         
         ## Running Unit Tests
         
         ```bash
         python setup.py test
         ```
         
@@ -121,15 +132,15 @@
         Generating *.mo file from *.po file. In root directory run command:
         ```bash
         msgfmt -o cron_descriptor/locale/YOUR_LOCALE_CODE.mo cron_descriptor/locale/YOUR_LOCALE_CODE.po
         ```
         
         ## Developing
         
-        All suggescions and PR's are welcomed
+        All suggestions and PR's are welcomed
         
         Just clone this repository and register pre-commit hook by running:
         
         ```bash
         ln -s ../../pre-commit.sh .git/hooks/pre-commit
         ```
         
@@ -144,15 +155,21 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.5
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `cron_descriptor-1.2.9/cron_descriptor/ExpressionDescriptor.py` & `cron_descriptor-1.3.0/cron_descriptor/ExpressionDescriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,121 +1,119 @@
-# Copyright (C) 2016 Adam Schubert <adam.schubert@sg1-game.net>
+# The MIT License (MIT)
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Copyright (c) 2016 Adam Schubert
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 
 import re
 import datetime
 import calendar
 
 from .GetText import GetText
 from .CasingTypeEnum import CasingTypeEnum
 from .DescriptionTypeEnum import DescriptionTypeEnum
 from .ExpressionParser import ExpressionParser
 from .Options import Options
 from .StringBuilder import StringBuilder
 from .Exception import FormatException, WrongArgumentException
 
 
-class ExpressionDescriptor(object):
+class ExpressionDescriptor:
 
     """
      Converts a Cron Expression into a human readable string
     """
 
     _special_characters = ['/', '-', ',', '*']
+
     _expression = ''
     _options = None
     _expression_parts = []
-    _parsed = False
 
     def __init__(self, expression, options=None, **kwargs):
-        """Initializes a new instance of the ExpressionDescriptorclass
+        """Initializes a new instance of the ExpressionDescriptor
 
         Args:
             expression: The cron expression string
             options: Options to control the output description
         Raises:
-            WrongArgumentException: if kwarg is unknow
+            WrongArgumentException: if kwarg is unknown
 
         """
         if options is None:
             options = Options()
         self._expression = expression
         self._options = options
         self._expression_parts = []
-        self._parsed = False
 
-        # if kwargs in _options, overwrite it, if not raise exeption
+        # if kwargs in _options, overwrite it, if not raise exception
         for kwarg in kwargs:
             if hasattr(self._options, kwarg):
                 setattr(self._options, kwarg, kwargs[kwarg])
             else:
-                raise WrongArgumentException(
-                    "Unknow {} configuration argument".format(kwarg))
+                raise WrongArgumentException("Unknown {} configuration argument".format(kwarg))
 
         # Initializes localization
-        GetText(options.locale_code)
+        self.get_text = GetText(options.locale_code, options.locale_location)
+
+        # Parse expression
+        parser = ExpressionParser(self._expression, self._options)
+        self._expression_parts = parser.parse()
+
+    def _(self, message):
+        return self.get_text.trans.gettext(message)
 
     def get_description(self, description_type=DescriptionTypeEnum.FULL):
-        """Generates a human readable string for the Cron Expression
+        """Generates a humanreadable string for the Cron Expression
 
         Args:
             description_type: Which part(s) of the expression to describe
-            options: Options to control the output description
         Returns:
             The cron expression description
         Raises:
-            Exception: if throw_exception_on_parse_error is True
+            Exception:
 
         """
-        try:
-            if self._parsed is False:
-                parser = ExpressionParser(self._expression, self._options)
-                self._expression_parts = parser.parse()
-                self._parsed = True
-
-            choices = {
-                DescriptionTypeEnum.FULL: self.get_full_description,
-                DescriptionTypeEnum.TIMEOFDAY: self.get_time_of_day_description,
-                DescriptionTypeEnum.HOURS: self.get_hours_description,
-                DescriptionTypeEnum.MINUTES: self.get_minutes_description,
-                DescriptionTypeEnum.SECONDS: self.get_seconds_description,
-                DescriptionTypeEnum.DAYOFMONTH: self.get_day_of_month_description,
-                DescriptionTypeEnum.MONTH: self.get_month_description,
-                DescriptionTypeEnum.DAYOFWEEK: self.get_day_of_week_description,
-                DescriptionTypeEnum.YEAR: self.get_year_description,
-            }
-
-            description = choices.get(description_type, self.get_seconds_description)()
-
-        except Exception as ex:
-            if self._options.throw_exception_on_parse_error:
-                raise
-            else:
-                description = str(ex)
-        return description
+        choices = {
+            DescriptionTypeEnum.FULL: self.get_full_description,
+            DescriptionTypeEnum.TIMEOFDAY: self.get_time_of_day_description,
+            DescriptionTypeEnum.HOURS: self.get_hours_description,
+            DescriptionTypeEnum.MINUTES: self.get_minutes_description,
+            DescriptionTypeEnum.SECONDS: self.get_seconds_description,
+            DescriptionTypeEnum.DAYOFMONTH: self.get_day_of_month_description,
+            DescriptionTypeEnum.MONTH: self.get_month_description,
+            DescriptionTypeEnum.DAYOFWEEK: self.get_day_of_week_description,
+            DescriptionTypeEnum.YEAR: self.get_year_description,
+        }
+
+        return choices.get(description_type, self.get_seconds_description)()
 
     def get_full_description(self):
         """Generates the FULL description
 
         Returns:
             The FULL description
         Raises:
-            FormatException: if formating fails and throw_exception_on_parse_error is True
+            FormatException: if formatting fails
 
         """
 
         try:
             time_segment = self.get_time_of_day_description()
             day_of_month_desc = self.get_day_of_month_description()
             month_desc = self.get_month_description()
@@ -125,24 +123,21 @@
             description = "{0}{1}{2}{3}{4}".format(
                 time_segment,
                 day_of_month_desc,
                 day_of_week_desc,
                 month_desc,
                 year_desc)
 
-            description = self.transform_verbosity(
-                description, self._options.verbose)
-            description = self.transform_case(
-                description,
-                self._options.casing_type)
+            description = self.transform_verbosity(description, self._options.verbose)
+            description = ExpressionDescriptor.transform_case(description, self._options.casing_type)
         except Exception:
-            description = _(
-                "An error occured when generating the expression description.  Check the cron expression syntax.")
-            if self._options.throw_exception_on_parse_error:
-                raise FormatException(description)
+            description = self._(
+                "An error occurred when generating the expression description.  Check the cron expression syntax."
+            )
+            raise FormatException(description)
 
         return description
 
     def get_time_of_day_description(self):
         """Generates a description for only the TIMEOFDAY portion of the expression
 
         Returns:
@@ -156,328 +151,368 @@
         description = StringBuilder()
 
         # handle special cases first
         if any(exp in minute_expression for exp in self._special_characters) is False and \
             any(exp in hour_expression for exp in self._special_characters) is False and \
                 any(exp in seconds_expression for exp in self._special_characters) is False:
             # specific time of day (i.e. 10 14)
-            description.append(_("At "))
+            description.append(self._("At "))
             description.append(
                 self.format_time(
                     hour_expression,
                     minute_expression,
                     seconds_expression))
-        elif "-" in minute_expression and \
+        elif seconds_expression == "" and "-" in minute_expression and \
             "," not in minute_expression and \
                 any(exp in hour_expression for exp in self._special_characters) is False:
             # minute range in single hour (i.e. 0-10 11)
             minute_parts = minute_expression.split('-')
-            description.append(_("Every minute between {0} and {1}").format(
+            description.append(self._("Every minute between {0} and {1}").format(
                 self.format_time(hour_expression, minute_parts[0]), self.format_time(hour_expression, minute_parts[1])))
-        elif "," in hour_expression and "-" not in hour_expression and \
+        elif seconds_expression == "" and "," in hour_expression and "-" not in hour_expression and \
                 any(exp in minute_expression for exp in self._special_characters) is False:
             # hours list with single minute (o.e. 30 6,14,16)
             hour_parts = hour_expression.split(',')
-            description.append(_("At"))
+            description.append(self._("At"))
             for i, hour_part in enumerate(hour_parts):
                 description.append(" ")
-                description.append(
-                    self.format_time(hour_part, minute_expression))
+                description.append(self.format_time(hour_part, minute_expression))
 
                 if i < (len(hour_parts) - 2):
                     description.append(",")
 
                 if i == len(hour_parts) - 2:
-                    description.append(_(" and"))
+                    description.append(self._(" and"))
         else:
             # default time description
             seconds_description = self.get_seconds_description()
             minutes_description = self.get_minutes_description()
             hours_description = self.get_hours_description()
 
             description.append(seconds_description)
 
-            if description:
+            if description and minutes_description:
                 description.append(", ")
 
             description.append(minutes_description)
 
-            if description:
+            if description and hours_description:
                 description.append(", ")
 
             description.append(hours_description)
         return str(description)
 
     def get_seconds_description(self):
         """Generates a description for only the SECONDS portion of the expression
 
         Returns:
             The SECONDS description
 
         """
 
+        def get_description_format(s):
+            if s == "0":
+                return ""
+
+            try:
+                if int(s) < 20:
+                    return self._("at {0} seconds past the minute")
+                else:
+                    return self._("at {0} seconds past the minute [grThen20]") or self._("at {0} seconds past the minute")
+            except ValueError:
+                return self._("at {0} seconds past the minute")
+
         return self.get_segment_description(
             self._expression_parts[0],
-            _("every second"),
+            self._("every second"),
             lambda s: s,
-            lambda s: _("every {0} seconds").format(s),
-            lambda s: _("seconds {0} through {1} past the minute"),
-            lambda s: _("at {0} seconds past the minute")
+            lambda s: self._("every {0} seconds").format(s),
+            lambda s: self._("seconds {0} through {1} past the minute"),
+            get_description_format,
+            lambda s: self._(", second {0} through second {1}") or self._(", {0} through {1}")
         )
 
     def get_minutes_description(self):
         """Generates a description for only the MINUTE portion of the expression
 
         Returns:
             The MINUTE description
 
         """
+        seconds_expression = self._expression_parts[0]
+
+        def get_description_format(s):
+            if s == "0" and seconds_expression == "":
+                return ""
+
+            try:
+                if int(s) < 20:
+                    return self._("at {0} minutes past the hour")
+                else:
+                    return self._("at {0} minutes past the hour [grThen20]") or self._("at {0} minutes past the hour")
+            except ValueError:
+                return self._("at {0} minutes past the hour")
 
         return self.get_segment_description(
             self._expression_parts[1],
-            _("every minute"),
+            self._("every minute"),
             lambda s: s,
-            lambda s: _("every {0} minutes").format(s),
-            lambda s: _("minutes {0} through {1} past the hour"),
-            lambda s: '' if s == "0" else _("at {0} minutes past the hour")
+            lambda s: self._("every {0} minutes").format(s),
+            lambda s: self._("minutes {0} through {1} past the hour"),
+            get_description_format,
+            lambda s: self._(", minute {0} through minute {1}") or self._(", {0} through {1}")
         )
 
     def get_hours_description(self):
         """Generates a description for only the HOUR portion of the expression
 
         Returns:
             The HOUR description
 
         """
         expression = self._expression_parts[2]
         return self.get_segment_description(
             expression,
-            _("every hour"),
+            self._("every hour"),
             lambda s: self.format_time(s, "0"),
-            lambda s: _("every {0} hours").format(s),
-            lambda s: _("between {0} and {1}"),
-            lambda s: _("at {0}")
+            lambda s: self._("every {0} hours").format(s),
+            lambda s: self._("between {0} and {1}"),
+            lambda s: self._("at {0}"),
+            lambda s: self._(", hour {0} through hour {1}") or self._(", {0} through {1}")
         )
 
     def get_day_of_week_description(self):
         """Generates a description for only the DAYOFWEEK portion of the expression
 
         Returns:
             The DAYOFWEEK description
 
         """
 
-        if self._expression_parts[5] == "*" and self._expression_parts[3] != "*":
-            # DOM is specified and DOW is * so to prevent contradiction like "on day 1 of the month, every day"
-            # we will not specified a DOW description.
+        if self._expression_parts[5] == "*":
+            # DOW is specified as * so we will not generate a description and defer to DOM part.
+            # Otherwise, we could get a contradiction like "on day 1 of the month, every day"
+            # or a dupe description like "every day, every day".
             return ""
 
         def get_day_name(s):
             exp = s
             if "#" in s:
-                exp, useless = s.split("#", 2)
+                exp, _ = s.split("#", 2)
             elif "L" in s:
                 exp = exp.replace("L", '')
-            return self.number_to_day(int(exp))
+            return ExpressionDescriptor.number_to_day(int(exp))
 
         def get_format(s):
             if "#" in s:
                 day_of_week_of_month = s[s.find("#") + 1:]
 
                 try:
-                    day_of_week_of_month_numer = int(day_of_week_of_month)
+                    day_of_week_of_month_number = int(day_of_week_of_month)
                     choices = {
-                        1: _("first"),
-                        2: _("second"),
-                        3: _("third"),
-                        4: _("forth"),
-                        5: _("fifth"),
+                        1: self._("first"),
+                        2: self._("second"),
+                        3: self._("third"),
+                        4: self._("forth"),
+                        5: self._("fifth"),
                     }
-                    day_of_week_of_month_description = choices.get(day_of_week_of_month_numer, None)
+                    day_of_week_of_month_description = choices.get(day_of_week_of_month_number, '')
                 except ValueError:
-                    day_of_week_of_month_description = None
+                    day_of_week_of_month_description = ''
 
-                formated = "{}{}{}".format(_(", on the "),
-                                           day_of_week_of_month_description, _(" {0} of the month"))
+                formatted = "{}{}{}".format(self._(", on the "), day_of_week_of_month_description, self._(" {0} of the month"))
             elif "L" in s:
-                formated = _(", on the last {0} of the month")
+                formatted = self._(", on the last {0} of the month")
             else:
-                formated = _(", only on {0}")
+                formatted = self._(", only on {0}")
 
-            return formated
+            return formatted
 
         return self.get_segment_description(
             self._expression_parts[5],
-            _(", every day"),
+            self._(", every day"),
             lambda s: get_day_name(s),
-            lambda s: _(", every {0} days of the week").format(s),
-            lambda s: _(", {0} through {1}"),
-            lambda s: get_format(s)
+            lambda s: self._(", every {0} days of the week").format(s),
+            lambda s: self._(", {0} through {1}"),
+            lambda s: get_format(s),
+            lambda s: self._(", {0} through {1}")
         )
 
     def get_month_description(self):
         """Generates a description for only the MONTH portion of the expression
 
         Returns:
             The MONTH description
 
         """
         return self.get_segment_description(
             self._expression_parts[4],
             '',
             lambda s: datetime.date(datetime.date.today().year, int(s), 1).strftime("%B"),
-            lambda s: _(", every {0} months").format(s),
-            lambda s: _(", {0} through {1}"),
-            lambda s: _(", only in {0}")
+            lambda s: self._(", every {0} months").format(s),
+            lambda s: self._(", month {0} through month {1}") or self._(", {0} through {1}"),
+            lambda s: self._(", only in {0}"),
+            lambda s: self._(", month {0} through month {1}") or self._(", {0} through {1}")
         )
 
     def get_day_of_month_description(self):
         """Generates a description for only the DAYOFMONTH portion of the expression
 
         Returns:
             The DAYOFMONTH description
 
         """
         expression = self._expression_parts[3]
-        expression = expression.replace("?", "*")
 
         if expression == "L":
-            description = _(", on the last day of the month")
+            description = self._(", on the last day of the month")
         elif expression == "LW" or expression == "WL":
-            description = _(", on the last weekday of the month")
+            description = self._(", on the last weekday of the month")
         else:
-            regex = re.compile("(\\d{1,2}W)|(W\\d{1,2})")
-            if regex.match(expression):
-                m = regex.match(expression)
+            regex = re.compile(r"(\d{1,2}W)|(W\d{1,2})")
+            m = regex.match(expression)
+            if m:  # if matches
                 day_number = int(m.group().replace("W", ""))
 
-                day_string = _("first weekday") if day_number == 1 else _("weekday nearest day {0}").format(
-                    day_number)
-                description = _(", on the {0} of the month").format(
-                    day_string)
+                day_string = self._("first weekday") if day_number == 1 else self._("weekday nearest day {0}").format(day_number)
+                description = self._(", on the {0} of the month").format(day_string)
             else:
-                description = self.get_segment_description(
-                    expression,
-                    _(", every day"),
-                    lambda s: s,
-                    lambda s: _(", every day") if s == "1" else _(", every {0} days"),
-                    lambda s: _(", between day {0} and {1} of the month"),
-                    lambda s: _(", on day {0} of the month")
-                )
+                # Handle "last day offset"(i.e.L - 5: "5 days before the last day of the month")
+                regex = re.compile(r"L-(\d{1,2})")
+                m = regex.match(expression)
+                if m:  # if matches
+                    off_set_days = m.group(1)
+                    description = self._(", {0} days before the last day of the month").format(off_set_days)
+                else:
+                    description = self.get_segment_description(
+                        expression,
+                        self._(", every day"),
+                        lambda s: s,
+                        lambda s: self._(", every day") if s == "1" else self._(", every {0} days"),
+                        lambda s: self._(", between day {0} and {1} of the month"),
+                        lambda s: self._(", on day {0} of the month"),
+                        lambda s: self._(", {0} through {1}")
+                    )
 
         return description
 
     def get_year_description(self):
         """Generates a description for only the YEAR portion of the expression
 
         Returns:
             The YEAR description
 
         """
 
         def format_year(s):
-            regex = re.compile("^\d+$")
+            regex = re.compile(r"^\d+$")
             if regex.match(s):
                 year_int = int(s)
                 if year_int < 1900:
                     return year_int
                 return datetime.date(year_int, 1, 1).strftime("%Y")
             else:
                 return s
 
         return self.get_segment_description(
             self._expression_parts[6],
             '',
             lambda s: format_year(s),
-            lambda s: _(", every {0} years").format(s),
-            lambda s: _(", {0} through {1}"),
-            lambda s: _(", only in {0}")
+            lambda s: self._(", every {0} years").format(s),
+            lambda s: self._(", year {0} through year {1}") or self._(", {0} through {1}"),
+            lambda s: self._(", only in {0}"),
+            lambda s: self._(", year {0} through year {1}") or self._(", {0} through {1}")
         )
 
     def get_segment_description(
         self,
         expression,
         all_description,
         get_single_item_description,
         get_interval_description_format,
         get_between_description_format,
-        get_description_format
+        get_description_format,
+        get_range_format
     ):
         """Returns segment description
         Args:
             expression: Segment to descript
             all_description: *
             get_single_item_description: 1
             get_interval_description_format: 1/2
             get_between_description_format: 1-2
             get_description_format: format get_single_item_description
+            get_range_format: function that formats range expressions depending on cron parts
         Returns:
             segment description
 
         """
         description = None
         if expression is None or expression == '':
             description = ''
         elif expression == "*":
             description = all_description
         elif any(ext in expression for ext in ['/', '-', ',']) is False:
-            description = get_description_format(expression).format(
-                get_single_item_description(expression))
+            description = get_description_format(expression).format(get_single_item_description(expression))
         elif "/" in expression:
             segments = expression.split('/')
-            description = get_interval_description_format(
-                segments[1]).format(get_single_item_description(segments[1]))
+            description = get_interval_description_format(segments[1]).format(get_single_item_description(segments[1]))
 
             # interval contains 'between' piece (i.e. 2-59/3 )
             if "-" in segments[0]:
                 between_segment_description = self.generate_between_segment_description(
-                    segments[0], get_between_description_format, get_single_item_description)
+                    segments[0],
+                    get_between_description_format,
+                    get_single_item_description
+                )
                 if not between_segment_description.startswith(", "):
                     description += ", "
+
                 description += between_segment_description
             elif any(ext in segments[0] for ext in ['*', ',']) is False:
                 range_item_description = get_description_format(segments[0]).format(
                     get_single_item_description(segments[0])
                 )
                 range_item_description = range_item_description.replace(", ", "")
 
-                description += _(", starting {0}").format(range_item_description)
+                description += self._(", starting {0}").format(range_item_description)
         elif "," in expression:
             segments = expression.split(',')
 
             description_content = ''
             for i, segment in enumerate(segments):
                 if i > 0 and len(segments) > 2:
                     description_content += ","
 
                     if i < len(segments) - 1:
                         description_content += " "
 
                 if i > 0 and len(segments) > 1 and (i == len(segments) - 1 or len(segments) == 2):
-                    description_content += _(" and ")
+                    description_content += self._(" and ")
 
                 if "-" in segment:
-                    between_description = self.generate_between_segment_description(
+                    between_segment_description = self.generate_between_segment_description(
                         segment,
-                        lambda s: _(", {0} through {1}"),
+                        get_range_format,
                         get_single_item_description
                     )
 
-                    between_description = between_description.replace(", ", "")
+                    between_segment_description = between_segment_description.replace(", ", "")
 
-                    description_content += between_description
+                    description_content += between_segment_description
                 else:
                     description_content += get_single_item_description(segment)
 
-            description = get_description_format(
-                expression).format(
-                    description_content)
+            description = get_description_format(expression).format(description_content)
         elif "-" in expression:
             description = self.generate_between_segment_description(
-                expression, get_between_description_format, get_single_item_description)
+                expression,
+                get_between_description_format,
+                get_single_item_description
+            )
 
         return description
 
     def generate_between_segment_description(
             self,
             between_expression,
             get_between_description_format,
@@ -490,108 +525,116 @@
         :param get_single_item_description:
         :return: The between segment description
         """
         description = ""
         between_segments = between_expression.split('-')
         between_segment_1_description = get_single_item_description(between_segments[0])
         between_segment_2_description = get_single_item_description(between_segments[1])
-        between_segment_2_description = between_segment_2_description.replace(
-            ":00", ":59")
+        between_segment_2_description = between_segment_2_description.replace(":00", ":59")
 
         between_description_format = get_between_description_format(between_expression)
         description += between_description_format.format(between_segment_1_description, between_segment_2_description)
 
         return description
 
     def format_time(
         self,
         hour_expression,
         minute_expression,
         second_expression=''
     ):
-        """Given time parts, will contruct a formatted time description
+        """Given time parts, will construct a formatted time description
         Args:
             hour_expression: Hours part
             minute_expression: Minutes part
             second_expression: Seconds part
         Returns:
             Formatted time description
 
         """
         hour = int(hour_expression)
 
         period = ''
         if self._options.use_24hour_time_format is False:
-            period = " PM" if (hour >= 12) else " AM"
+            period = self._("PM") if (hour >= 12) else self._("AM")
+            if period:
+                # add preceding space
+                period = " " + period
+
             if hour > 12:
                 hour -= 12
 
-        minute = str(int(minute_expression))  # !FIXME WUT ???
+            if hour == 0:
+                hour = 12
+
+        minute = str(int(minute_expression))  # Removes leading zero if any
         second = ''
         if second_expression is not None and second_expression:
             second = "{}{}".format(":", str(int(second_expression)).zfill(2))
 
         return "{0}:{1}{2}{3}".format(str(hour).zfill(2), minute.zfill(2), second, period)
 
     def transform_verbosity(self, description, use_verbose_format):
         """Transforms the verbosity of the expression description by stripping verbosity from original description
         Args:
             description: The description to transform
             use_verbose_format: If True, will leave description as it, if False, will strip verbose parts
-            second_expression: Seconds part
         Returns:
             The transformed description with proper verbosity
 
         """
         if use_verbose_format is False:
-            description = description.replace(
-                _(", every minute"), '')
-            description = description.replace(_(", every hour"), '')
-            description = description.replace(_(", every day"), '')
+            description = description.replace(self._(", every minute"), '')
+            description = description.replace(self._(", every hour"), '')
+            description = description.replace(self._(", every day"), '')
+            description = re.sub(r', ?$', '', description)
         return description
 
-    def transform_case(self, description, case_type):
+    @staticmethod
+    def transform_case(description, case_type):
         """Transforms the case of the expression description, based on options
         Args:
             description: The description to transform
             case_type: The casing type that controls the output casing
-            second_expression: Seconds part
         Returns:
             The transformed description with proper casing
-
         """
         if case_type == CasingTypeEnum.Sentence:
             description = "{}{}".format(
                 description[0].upper(),
                 description[1:])
         elif case_type == CasingTypeEnum.Title:
             description = description.title()
         else:
             description = description.lower()
         return description
 
-    def number_to_day(self, day_number):
+    @staticmethod
+    def number_to_day(day_number):
         """Returns localized day name by its CRON number
 
         Args:
             day_number: Number of a day
         Returns:
             Day corresponding to day_number
         Raises:
             IndexError: When day_number is not found
         """
-        return [
-            calendar.day_name[6],
-            calendar.day_name[0],
-            calendar.day_name[1],
-            calendar.day_name[2],
-            calendar.day_name[3],
-            calendar.day_name[4],
-            calendar.day_name[5]
-        ][day_number]
+        try:
+            return [
+                calendar.day_name[6],
+                calendar.day_name[0],
+                calendar.day_name[1],
+                calendar.day_name[2],
+                calendar.day_name[3],
+                calendar.day_name[4],
+                calendar.day_name[5]
+            ][day_number]
+        except IndexError:
+            raise IndexError("Day {} is out of range!".format(day_number))
 
     def __str__(self):
         return self.get_description()
 
     def __repr__(self):
         return self.get_description()
```

### Comparing `cron_descriptor-1.2.9/cron_descriptor/ExpressionParser.py` & `cron_descriptor-1.3.0/cron_descriptor/ExpressionParser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-# Copyright (C) 2016 Adam Schubert <adam.schubert@sg1-game.net>
+# The MIT License (MIT)
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Copyright (c) 2016 Adam Schubert
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 
 import re
 
 from .Exception import MissingFieldException, FormatException
 
 
 class ExpressionParser(object):
-
-    """
-     Parses and validates a Cron Expression into list of fixed len()
-    """
-
     _expression = ''
     _options = None
 
     _cron_days = {
         0: 'SUN',
         1: 'MON',
         2: 'TUE',
@@ -77,85 +79,97 @@
             raise MissingFieldException("ExpressionDescriptor.expression")
         else:
             expression_parts_temp = self._expression.split()
             expression_parts_temp_length = len(expression_parts_temp)
             if expression_parts_temp_length < 5:
                 raise FormatException(
                     "Error: Expression only has {0} parts.  At least 5 part are required.".format(
-                        expression_parts_temp_length))
+                        expression_parts_temp_length
+                    )
+                )
             elif expression_parts_temp_length == 5:
                 # 5 part cron so shift array past seconds element
                 for i, expression_part_temp in enumerate(expression_parts_temp):
                     parsed[i + 1] = expression_part_temp
             elif expression_parts_temp_length == 6:
-                # If last element ends with 4 digits, a year element has been
-                # supplied and no seconds element
-                year_regex = re.compile("\d{4}$")
-                if year_regex.search(expression_parts_temp[5]) is not None:
-                    for i, expression_part_temp in enumerate(expression_parts_temp):
+                # We will detect if this 6 part expression has a year specified and if so we will shift the parts and treat the
+                # first part as a minute part rather than a second part.
+                # Ways we detect:
+                # 1. Last part is a literal year (i.e. 2020)
+                # 2. 3rd or 5th part is specified as "?" (DOM or DOW)
+                year_regex = re.compile(r"\d{4}$")
+                is_year_with_no_seconds_part = bool(year_regex.search(expression_parts_temp[5])) or "?" in [expression_parts_temp[4], expression_parts_temp[2]]
+                for i, expression_part_temp in enumerate(expression_parts_temp):
+                    if is_year_with_no_seconds_part:
+                        # Shift parts over by one
                         parsed[i + 1] = expression_part_temp
-                else:
-                    for i, expression_part_temp in enumerate(expression_parts_temp):
+                    else:
                         parsed[i] = expression_part_temp
+
             elif expression_parts_temp_length == 7:
                 parsed = expression_parts_temp
             else:
                 raise FormatException(
                     "Error: Expression has too many parts ({0}).  Expression must not have more than 7 parts.".format(
-                        expression_parts_temp_length))
+                        expression_parts_temp_length
+                    )
+                )
         self.normalize_expression(parsed)
 
         return parsed
 
-    """
-
-    @param:
-    """
-
     def normalize_expression(self, expression_parts):
         """Converts cron expression components into consistent, predictable formats.
         Args:
             expression_parts: A 7 part string array, one part for each component of the cron expression
         Returns:
             None
         """
         # convert ? to * only for DOM and DOW
         expression_parts[3] = expression_parts[3].replace("?", "*")
         expression_parts[5] = expression_parts[5].replace("?", "*")
 
         # convert 0/, 1/ to */
         if expression_parts[0].startswith("0/"):
-            expression_parts[0] = expression_parts[
-                0].replace("0/", "*/")  # seconds
+            expression_parts[0] = expression_parts[0].replace("0/", "*/")  # seconds
 
         if expression_parts[1].startswith("0/"):
-            expression_parts[1] = expression_parts[
-                1].replace("0/", "*/")  # minutes
+            expression_parts[1] = expression_parts[1].replace("0/", "*/")  # minutes
 
         if expression_parts[2].startswith("0/"):
-            expression_parts[2] = expression_parts[
-                2].replace("0/", "*/")  # hours
+            expression_parts[2] = expression_parts[2].replace("0/", "*/")  # hours
 
         if expression_parts[3].startswith("1/"):
             expression_parts[3] = expression_parts[3].replace("1/", "*/")  # DOM
 
         if expression_parts[4].startswith("1/"):
-            expression_parts[4] = expression_parts[
-                4].replace("1/", "*/")  # Month
+            expression_parts[4] = expression_parts[4].replace("1/", "*/")  # Month
 
         if expression_parts[5].startswith("1/"):
             expression_parts[5] = expression_parts[5].replace("1/", "*/")  # DOW
 
         if expression_parts[6].startswith("1/"):
-            expression_parts[6] = expression_parts[6].replace("1/", "*/")
+            expression_parts[6] = expression_parts[6].replace("1/", "*/")  # Years
+
+        # Adjust DOW based on dayOfWeekStartIndexZero option
+        def digit_replace(match):
+            match_value = match.group()
+            dow_digits = re.sub(r'\D', "", match_value)
+            dow_digits_adjusted = dow_digits
+            if self._options.day_of_week_start_index_zero:
+                if dow_digits == "7":
+                    dow_digits_adjusted = "0"
+            else:
+                dow_digits_adjusted = str(int(dow_digits) - 1)
 
-        # handle DayOfWeekStartIndexZero option where SUN=1 rather than SUN=0
-        if self._options.day_of_week_start_index_zero is False:
-            expression_parts[5] = self.decrease_days_of_week(expression_parts[5])
+            return match_value.replace(dow_digits, dow_digits_adjusted)
 
+        expression_parts[5] = re.sub(r'(^\d)|([^#/\s]\d)', digit_replace, expression_parts[5])
+
+        # Convert DOM '?' to '*'
         if expression_parts[3] == "?":
             expression_parts[3] = "*"
 
         # convert SUN-SAT format to 0-6 format
         for day_number in self._cron_days:
             expression_parts[5] = expression_parts[5].upper().replace(self._cron_days[day_number], str(day_number))
 
@@ -164,14 +178,26 @@
             expression_parts[4] = expression_parts[4].upper().replace(
                 self._cron_months[month_number], str(month_number))
 
         # convert 0 second to (empty)
         if expression_parts[0] == "0":
             expression_parts[0] = ''
 
+        # If time interval is specified for seconds or minutes and next time part is single item, make it a "self-range" so
+        # the expression can be interpreted as an interval 'between' range.
+        # For example:
+        # 0-20/3 9 * * * => 0-20/3 9-9 * * * (9 => 9-9)
+        # */5 3 * * * => */5 3-3 * * * (3 => 3-3)
+        star_and_slash = ['*', '/']
+        has_part_zero_star_and_slash = any(ext in expression_parts[0] for ext in star_and_slash)
+        has_part_one_star_and_slash = any(ext in expression_parts[1] for ext in star_and_slash)
+        has_part_two_special_chars = any(ext in expression_parts[2] for ext in ['*', '-', ',', '/'])
+        if not has_part_two_special_chars and (has_part_zero_star_and_slash or has_part_one_star_and_slash):
+            expression_parts[2] += '-{}'.format(expression_parts[2])
+
         # Loop through all parts and apply global normalization
         length = len(expression_parts)
         for i in range(length):
 
             # convert all '*/1' to '*'
             if expression_parts[i] == "*/1":
                 expression_parts[i] = "*"
@@ -181,30 +207,19 @@
             This allows us to reuse the between expression handling for step values.
 
             For Example:
             - month part '3/2' will be converted to '3-12/2' (every 2 months between March and December)
             - DOW part '3/2' will be converted to '3-6/2' (every 2 days between Tuesday and Saturday)
             """
 
-            if "/" in expression_parts[i] and any(exp in expression_parts[i] for exp in ['*', '-', ',']) is False:
+            if "/" in expression_parts[i] and not any(exp in expression_parts[i] for exp in ['*', '-', ',']):
                 choices = {
                     4: "12",
                     5: "6",
                     6: "9999"
                 }
 
                 step_range_through = choices.get(i)
 
                 if step_range_through is not None:
                     parts = expression_parts[i].split('/')
                     expression_parts[i] = "{0}-{1}/{2}".format(parts[0], step_range_through, parts[1])
-
-    def decrease_days_of_week(self, day_of_week_expression_part):
-        dow_chars = list(day_of_week_expression_part)
-        for i, dow_char in enumerate(dow_chars):
-            if i == 0 or dow_chars[i - 1] != '#' and dow_chars[i - 1] != '/':
-                try:
-                    char_numeric = int(dow_char)
-                    dow_chars[i] = str(char_numeric - 1)[0]
-                except ValueError:
-                    pass
-        return ''.join(dow_chars)
```

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/tr_TR.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/tr_TR.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/zh_CN.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/zh_CN.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/pt_PT.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/pt_PT.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/sv_SE.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/sv_SE.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/fr_FR.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/fr_FR.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/ru_RU.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/ru_RU.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/it_IT.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/it_IT.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/uk_UA.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/uk_UA.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/nb_NO.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/nb_NO.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/de_DE.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/de_DE.mo`

 * *Files identical despite different names*

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/nl_NL.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/nl_NL.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: 1.0\n"
 "Report-Msgid-Bugs-To: adam.schubert@sg1-game.net\n"
-"POT-Creation-Date: 2016-01-19 02:00+0100\n"
 "PO-Revision-Date: 2016-01-19 02:00+0100\n"
 "Last-Translator: Adam Schubert <adam.schubert@sg1-game.net>\n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nl_NL\n"
@@ -75,18 +74,18 @@
 "An error occured when generating the expression description.  Check the cron "
 "expression syntax."
 msgstr ""
 "Er is een fout opgetreden bij het vertalen van de gegevens. Controleer de "
 "gegevens."
 
 msgid "At"
-msgstr "Op"
+msgstr "Om"
 
 msgid "At "
-msgstr "Op "
+msgstr "Om "
 
 msgid "Every minute between {0} and {1}"
 msgstr "Elke minuut tussen {0} en {1}"
 
 msgid "at {0}"
 msgstr "op {0}"
```

### Comparing `cron_descriptor-1.2.9/cron_descriptor/locale/cs_CZ.mo` & `cron_descriptor-1.3.0/cron_descriptor/locale/cs_CZ.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: 1.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-01-19 02:00+0100\n"
-"PO-Revision-Date: 2016-01-19 03:04+0100\n"
+"PO-Revision-Date: 2022-06-29 23:06+0200\n"
+"Last-Translator: Adam Schubert <adam.schubert@sg1-game.net>\n"
+"Language-Team: \n"
+"Language: cs_CZ\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: cs_CZ\n"
-"Last-Translator: Adam Schubert <adam.schubert@sg1-game.net>\n"
-"Language-Team: \n"
-"X-Generator: Poedit 1.8.4\n"
+"X-Generator: Poedit 3.0.1\n"
 
 msgid " and"
 msgstr " a"
 
 msgid " and "
 msgstr " a "
 
@@ -45,15 +44,15 @@
 msgid ", every {0} years"
 msgstr ", každý {0} rok"
 
 msgid ", on day {0} of the month"
 msgstr ", v {0} den v měsíci"
 
 msgid ", on the "
-msgstr ", na"
+msgstr ", na "
 
 msgid ", on the last day of the month"
 msgstr ", v poslední den měsíce"
 
 msgid ", on the last weekday of the month"
 msgstr ", v poslední všední den v měsíci"
 
@@ -96,21 +95,21 @@
 msgid "at {0} seconds past the minute"
 msgstr "v {0} sekund uplynulou minutu"
 
 msgid "between {0} and {1}"
 msgstr "mezi {0} a {1}"
 
 msgid "every hour"
-msgstr "Každou hodinu"
+msgstr "každou hodinu"
 
 msgid "every minute"
 msgstr "každou minutu"
 
 msgid "every second"
-msgstr "Každou sekundu"
+msgstr "každou sekundu"
 
 msgid "every {0} hours"
 msgstr "každých {0} hodin"
 
 msgid "every {0} minutes"
 msgstr "každých {0} minut"
 
@@ -126,15 +125,15 @@
 msgid "first weekday"
 msgstr "první víkendový den"
 
 msgid "forth"
 msgstr "čtvrtý"
 
 msgid "minutes {0} through {1} past the hour"
-msgstr "{0} až {1} minut "
+msgstr "{0} až {1} minut"
 
 msgid "second"
 msgstr "druhý"
 
 msgid "seconds {0} through {1} past the minute"
 msgstr "{0} až {1}  sekund"
```

### Comparing `cron_descriptor-1.2.9/PKG-INFO` & `cron_descriptor-1.3.0/cron_descriptor.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,115 @@
-Metadata-Version: 1.1
-Name: cron_descriptor
-Version: 1.2.9
+Metadata-Version: 2.1
+Name: cron-descriptor
+Version: 1.3.0
 Summary: A Python library that converts cron expressions into human readable strings.
 Home-page: https://github.com/Salamek/cron-descriptor
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: UNKNOWN
 Description: # Cron Descriptor
         
-        Master: [![Master Build Status](https://api.travis-ci.org/Salamek/cron-descriptor.svg?branch=master)](https://travis-ci.org/Salamek/cron-descriptor) All: [![Build Status](https://api.travis-ci.org/Salamek/cron-descriptor.svg)](https://travis-ci.org/Salamek/cron-descriptor)
-        [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=D8LQ4XTBLV3C4&lc=CZ&item_number=Salamekcron-descriptor&currency_code=EUR)
+        [![Python tests](https://github.com/Salamek/cron-descriptor/actions/workflows/python-test.yml/badge.svg)](https://github.com/Salamek/cron-descriptor/actions/workflows/python-test.yml)
+        [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/salamek)
         
         A Python library that converts cron expressions into human readable strings. Ported to Python from https://github.com/bradyholt/cron-expression-descriptor.
         
         **Author**: Adam Schubert (https://www.salamek.cz)  
         **Original Author & Credit**: Brady Holt (http://www.geekytidbits.com)  
         **License**: [MIT](http://opensource.org/licenses/MIT)
         
         ## Features         
          * Supports all cron expression special characters including * / , - ? L W, #
          * Supports 5, 6 (w/ seconds or year), or 7 (w/ seconds and year) part cron expressions
          * Provides casing options (Sentence, Title, Lower, etc.)
-         * Localization with support for 14 languages
-         * Supports Python 2.7 - 3.4
+         * Localization with support for 17 languages
+         * Supports Python 2.7 - 3.10
         
         ## Installation
         Using PIP
         ```bash
         pip install cron-descriptor
         ```
         
         ## Usage example
         
+        ### Simple
         ```python
-        # Simple
         from cron_descriptor import get_description, ExpressionDescriptor
         
         print(get_description("* 2 3 * *"))
         
         #OR
         
         print(str(ExpressionDescriptor("* 2 3 * *")))
         ```
         
+        ### Advanced
         ```python
-        # Advanced
         # Consult Options.py/CasingTypeEnum.py/DescriptionTypeEnum.py for more info
         from cron_descriptor import Options, CasingTypeEnum, DescriptionTypeEnum, ExpressionDescriptor
         
-        descripter = ExpressionDescriptor("*/10 * * * *", throw_exception_on_parse_error = True, casing_type = CasingTypeEnum.Sentence, use_24hour_time_format = True)
+        descriptor = ExpressionDescriptor(
+            expression = "*/10 * * * *",
+            casing_type = CasingTypeEnum.Sentence,
+            use_24hour_time_format = True
+        )
+        
         # GetDescription uses DescriptionTypeEnum.FULL by default:
-        print(descripter.get_description())
-        print("{}".format(descripter))
+        print(descriptor.get_description())
+        print("{}".format(descriptor))
         
-        #or passing Options class as second argument:
+        # Or passing Options class as second argument:
         
         options = Options()
-        options.throw_exception_on_parse_error = True
         options.casing_type = CasingTypeEnum.Sentence
         options.use_24hour_time_format = True
-        descripter = ExpressionDescriptor("*/10 * * * *", options)
-        print(descripter.get_description(DescriptionTypeEnum.FULL))
-        
+        descriptor = ExpressionDescriptor("*/10 * * * *", options)
+        print(descriptor.get_description(DescriptionTypeEnum.FULL))
         ```
         
         ## Languages Available
-          * English ([Brady Holt](https://github.com/bradyholt))
-          * Brazilian ([Renato Lima](https://github.com/natenho))
-          * Spanish ([Ivan Santos](https://github.com/ivansg))
-          * Norwegian ([Siarhei Khalipski](https://github.com/KhalipskiSiarhei))
-          * Turkish ([Mustafa SADEDİL](https://github.com/sadedil))
-          * Dutch ([TotalMace](https://github.com/TotalMace))
-          * Chinese Simplified ([Star Peng](https://github.com/starpeng))
-          * Russian ([LbISS](https://github.com/LbISS))
-          * French ([Arnaud TAMAILLON](https://github.com/Greybird))
-          * German ([Michael Schuler](https://github.com/mschuler))
-          * Ukrainian ([Taras](https://github.com/tbudurovych))
-          * Italian ([rinaldihno](https://github.com/rinaldihno))
-          * Czech ([Adam Schubert](https://github.com/salamek))
-          * Swedish ([Åke Engelbrektson](https://github.com/eson57))
+        
+        |Language| Locale Code | Contributor |
+        |--------|-------------|-------------|
+        |English |en|[Brady Holt](https://github.com/bradyholt)|
+        |Brazilian |pt_PT|[Renato Lima](https://github.com/natenho)|
+        |Chinese Simplified | zh_CN |[Star Peng](https://github.com/starpeng)|
+        |Spanish |es_ES|[Ivan Santos](https://github.com/ivansg)|
+        |Norwegian |nb_NO|[Siarhei Khalipski](https://github.com/KhalipskiSiarhei)|
+        |Turkish |tr_TR|[Mustafa SADEDİL](https://github.com/sadedil)|
+        |Dutch |nl_NL|[TotalMace](https://github.com/TotalMace)|
+        |Russian |ru_RU|[LbISS](https://github.com/LbISS)|
+        |French |fr_FR|[Arnaud TAMAILLON](https://github.com/Greybird)|
+        |German |de_DE|[Michael Schuler](https://github.com/mschuler)|
+        |Ukrainian |uk_UA|[Taras](https://github.com/tbudurovych)|
+        |Italian |it_IT|[rinaldihno](https://github.com/rinaldihno)|
+        |Czech |cs_CZ|[Adam Schubert](https://github.com/salamek)|
+        |Swedish |sv_SE|[Åke Engelbrektson](https://github.com/eson57)|
+        |Tamil |ta_IN|[Sankar Hari](https://github.com/sankarhari)|
+        |Persian|fa_IR|[M. Yas. Davoodeh](https://github.com/Davoodeh)|
+        |Korean|ko_KR|[KyuJoo Han](https://github.com/hanqyu)|
+        |Japanese |ja_JP|[Tho Nguyen](https://github.com/tho-asterist)|
         
         <!-- SOON
         ## Demo
         
         
         
         ## Download
         
         -->
         
         ## Original Source
          - .NET - [https://github.com/bradyholt/cron-expression-descriptor](https://github.com/bradyholt/cron-expression-descriptor)
         
         ## Ports
-         - Java - [https://github.com/RedHogs/cron-parser](https://github.com/RedHogs/cron-parser)
-         - Ruby - [https://github.com/alpinweis/cronex](https://github.com/alpinweis/cronex)
+         - Java     - [https://github.com/RedHogs/cron-parser](https://github.com/RedHogs/cron-parser)
+         - Ruby     - [https://github.com/alpinweis/cronex](https://github.com/alpinweis/cronex)
+         - Golang   - [https://github.com/jsuar/go-cron-descriptor](https://github.com/jsuar/go-cron-descriptor)
         
         ## Running Unit Tests
         
         ```bash
         python setup.py test
         ```
         
@@ -121,15 +132,15 @@
         Generating *.mo file from *.po file. In root directory run command:
         ```bash
         msgfmt -o cron_descriptor/locale/YOUR_LOCALE_CODE.mo cron_descriptor/locale/YOUR_LOCALE_CODE.po
         ```
         
         ## Developing
         
-        All suggescions and PR's are welcomed
+        All suggestions and PR's are welcomed
         
         Just clone this repository and register pre-commit hook by running:
         
         ```bash
         ln -s ../../pre-commit.sh .git/hooks/pre-commit
         ```
         
@@ -144,15 +155,21 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.5
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

