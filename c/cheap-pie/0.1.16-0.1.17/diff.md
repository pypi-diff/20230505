# Comparing `tmp/cheap_pie-0.1.16.tar.gz` & `tmp/cheap_pie-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-0.1.16.tar", last modified: Sat Dec 10 02:26:09 2022, max compression
+gzip compressed data, was "cheap_pie-0.1.17.tar", last modified: Fri May  5 18:22:39 2023, max compression
```

## Comparing `cheap_pie-0.1.16.tar` & `cheap_pie-0.1.17.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.362281 cheap_pie-0.1.16/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.1.16/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2022-12-10 02:26:09.362458 cheap_pie-0.1.16/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6508 2022-12-10 01:01:26.000000 cheap_pie-0.1.16/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2022-12-10 02:26:09.364278 cheap_pie-0.1.16/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)      786 2022-12-10 02:23:26.000000 cheap_pie-0.1.16/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.273884 cheap_pie-0.1.16/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.283258 cheap_pie-0.1.16/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.308528 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7391 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2259 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cheap_pie.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2736 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1694 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5636 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     9105 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2373 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.320580 cheap_pie-0.1.16/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1568 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3862 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3728 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      315 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/name_subs.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      833 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3944 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3996 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.344033 cheap_pie-0.1.16/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1402 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/rdl2verilog.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/reload_module.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2275 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/search.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/tools/test_rdl.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.360121 cheap_pie-0.1.16/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3992 2022-12-10 02:06:51.000000 cheap_pie-0.1.16/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:26:09.294890 cheap_pie-0.1.16/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2022-12-10 02:26:09.000000 cheap_pie-0.1.16/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2022-12-10 02:26:09.000000 cheap_pie-0.1.16/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2022-12-10 02:26:09.000000 cheap_pie-0.1.16/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      129 2022-12-10 02:26:09.000000 cheap_pie-0.1.16/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2022-12-10 02:26:09.000000 cheap_pie-0.1.16/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.770849 cheap_pie-0.1.17/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.1.17/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-05 18:22:39.771406 cheap_pie-0.1.17/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7746 2023-05-05 18:19:03.000000 cheap_pie-0.1.17/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-05 18:22:39.772809 cheap_pie-0.1.17/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      808 2023-05-05 18:21:58.000000 cheap_pie-0.1.17/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.672416 cheap_pie-0.1.17/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.683720 cheap_pie-0.1.17/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.715144 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7755 2023-05-04 20:02:54.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2259 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cheap_pie.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2736 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1694 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5636 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     9105 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2235 2022-12-12 23:16:24.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.737000 cheap_pie-0.1.17/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1809 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3934 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3518 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      315 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/name_subs.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      910 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4016 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4068 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.752882 cheap_pie-0.1.17/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.1.17/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/rdl2verilog.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/reload_module.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2275 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/search.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/test_rdl.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.768229 cheap_pie-0.1.17/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4811 2022-12-12 23:20:40.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.694728 cheap_pie-0.1.17/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      139 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-0.1.16/LICENSE` & `cheap_pie-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/setup.py` & `cheap_pie-0.1.17/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='0.1.16',
+    version='0.1.17',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     url='https://github.com/bat52/cheap_pie',
@@ -23,9 +23,10 @@
           'esptool',
           'python-docx',
           'pyverilator',
           'peakrdl-ipxact',
           'peakrdl-uvm',
           'peakrdl-verilog',
           'hickle',
+          'packaging'
       ],
 )
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,15 +163,19 @@
             fieldval = (abs(fieldval) ^ (self.mask >> self.lsb)) + 1
 
         ## compute new register value ##################################################
         
         shiftval= fieldval << self.lsb
         maskinv= self.mask ^ literal_eval('0xFFFFFFFF')
         regmasked = regval & maskinv
-        outregval = regmasked + shiftval
+        outregval = regmasked + (shiftval & self.mask)
+
+        # check new value in range
+        if (shiftval & self.mask) < shiftval:
+            raise ValueError(f'Bitifield value f{fieldval} out of range!')
     
         ## write back new register value ###############################################
         if writeback:
             self.hif.hifwrite(self.addr,outregval,*args,**kwargs)
         
         if echo:
             outstr=self._strval(fieldval)
@@ -241,10 +245,17 @@
 
     # options
     f.setbit(val,echo=True)
     f.setbit(val,writeback=False)
     rv = f.setbit(1,regval=1)
     assert(rv==5)
 
+    # test assertion
+    try:
+        f.setbit(7)
+        assert False, 'Assertion was not raised!!!'
+    except ValueError as error:
+        print('Assertion raised correctly: <%s>' % error)
+
 if __name__ == '__main__':
     test_cp_bitfield()    
     pass
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cheap_pie.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cheap_pie.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,17 @@
         from transport.cp_pyocd_transport import test_cp_pyocd
         test_cp_pyocd()
 
         # esptool
         from transport.cp_esptool_transport import test_cp_esptool
         test_cp_esptool()
 
-        if False:
-            # pyverilator 
-            from transport.cp_pyverilator_transport import test_cp_pyverilator
-            test_cp_pyverilator()
-        else:
-            print('Warning: pyverilator not working anymore after updating to ubuntu 22.04.')
+        # pyverilator 
+        from transport.cp_pyverilator_transport import test_cp_pyverilator
+        test_cp_pyverilator()
 
         pass
    
     def test_bitfield(self):
         from cheap_pie_core.cbitfield import test_cp_bitfield
         test_cp_bitfield()
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-0.1.17/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 e._name = e._name.replace(r,'')
             # remove recursively
             ipxact_remove_prefix(e)
 
     return ipx
     pass
 
-def ipxact_parse(fname,hif=None):
+def ipxact_parse(fname,hif=None, base_address_offset = "0x00000000"):
        
     ## read input file ########################################################
     csv = untangle.parse(fname)
 
     ## remove ipxact/spirit prefixes ##########################################
     csv = ipxact_remove_prefix(csv)
     
@@ -60,15 +60,15 @@
                 # new register
                 periph_name=periph.name.cdata
                 rname=reg.name.cdata
                 regname = "%s_%s" % ( periph_name,rname )
                 regname=name_subs(regname)
 
                 addr_str=reg.addressOffset.cdata.replace("'h",'0x')
-                regaddr=literal_eval(addr_str) + base_address
+                regaddr=literal_eval(addr_str) + base_address + literal_eval(base_address_offset)
                 comments=""
                 # print(comments)
                 struct_register=cp_register(regname,regaddr,comments,hif)
 
                 # for field_idx in range(nfields):
                 if hasattr(reg,'field'):
                     for field in reg.field :
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-0.1.17/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,47 +14,43 @@
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
 
-def ipxact_parse(fname,hif=None):
+def ipxact_parse(fname,hif=None, base_address_offset = "0x00000000"):
        
     ## read input file ########################################################
     xml = Component()
     xml.load(fname)
     
     ## loop over lines ########################################################
     outdict = dict()
 
     for m in xml.memoryMaps.memoryMap:
         for periph in m.addressBlock:
             # print(periph)
         
-            # base_addr_str=periph.baseAddress # .cdata.replace("'h",'0x')
-            # print(base_addr_str)
-            base_address=periph.baseAddress # literal_eval(base_addr_str)
+            base_address=periph.baseAddress
 
             if hasattr(periph,'register'):
                 for reg in periph.register:                
                     # close old register, before opening a new one
                     if 'regname' in locals():
                         struct_register.dictfield2struct()
                         outdict[regname]=struct_register
 
                     # new register
                     periph_name=periph.name
                     rname=reg.name
                     regname = "%s_%s" % ( periph_name,rname )
                     regname=name_subs(regname)
 
-                    # addr_str=reg.addressOffset.cdata.replace("'h",'0x')
-                    # regaddr=literal_eval(addr_str) + base_address
-                    regaddr=reg.addressOffset + base_address
+                    regaddr=reg.addressOffset + base_address + literal_eval(base_address_offset)
                     comments=reg.description
                     # print(comments)
                     struct_register=cp_register(regname,regaddr,comments,hif)
 
                     # for field_idx in range(nfields):
                     if hasattr(reg,'field'):
                         for field in reg.field :
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/parsers/rdl_parse.py` & `cheap_pie-0.1.17/src/cheap_pie/parsers/rdl_parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import sys
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from parsers.ipyxact_parse import ipxact_parse
 from tools.rdl2any import rdl2any
 
-def rdl_parse(fname,hif=None):
+def rdl_parse(fname,hif=None,base_address_offset = "0x00000000" ):
     # convert rdl to ipxact
     ipxact_fname = rdl2any(['-f',fname,'-ofmt','ipxact'])
     # parse ipxact
-    return ipxact_parse(ipxact_fname,hif=hif)    
+    return ipxact_parse(ipxact_fname,hif=hif, base_address_offset=base_address_offset)    
 
 def test_rdl_parse():
     rdl_parse("./devices/rdl/basic.rdl")
     rdl_parse("./devices/rdl/counter.rdl")
     pass
     
 if __name__ == '__main__':
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
     
-def svd_parse(fname,vendor=None,hif=None):
+def svd_parse(fname,vendor=None,hif=None, base_address_offset = "0x00000000"):
         
     ## read input file ########################################################
     svd = untangle.parse(fname)
     
     ## loop over lines ########################################################
     outdict = dict()
 
@@ -54,15 +54,15 @@
                     # new register
                     periph_name=periph.name.cdata
                     rname=reg.name.cdata
                     regname = "%s_%s" % ( periph_name,rname )
                     regname=name_subs(regname)
 
                     addr_str=reg.addressOffset.cdata
-                    regaddr=literal_eval(addr_str) + base_address
+                    regaddr=literal_eval(addr_str) + base_address + literal_eval(base_address_offset)
                     comments=reg.description.cdata
                     # print(comments)
                     struct_register=cp_register(regname,regaddr,comments,hif)
 
                     # for field_idx in range(nfields):
                     if hasattr(reg,'fields'):
                         for field in reg.fields.field :
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
     
-def svd_parse(fname,vendor=None,hif=None):
+def svd_parse(fname,vendor=None,hif=None, base_address_offset = "0x00000000"):
         
     ## read input file ########################################################
     if vendor is None:
         svd = SVDParser.for_xml_file(fname)
     else:
         svd = SVDParser.for_packaged_svd(vendor,fname)
 
@@ -55,15 +55,15 @@
 
                     # new register
                     periph_name=periph.name
                     rname=reg.name
                     regname = "%s_%s" % ( periph_name,rname )
                     regname=name_subs(regname)
 
-                    regaddr=reg.address_offset + base_address
+                    regaddr=reg.address_offset + base_address + literal_eval(base_address_offset)
                     comments=reg.description
                     # print(comments)
                     struct_register=cp_register(regname,regaddr,comments,hif)
 
                     # for field_idx in range(nfields):
                     if hasattr(reg,'fields'):
                         for field in reg.fields :
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-0.1.17/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-0.1.17/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-0.1.17/src/cheap_pie/tools/rdl2any.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 #!/usr/bin/python3
 
 import sys
 import os
-from systemrdl import RDLCompiler, RDLCompileError
-from peakrdl.verilog import VerilogExporter
-from peakrdl_ipxact import IPXACTExporter
-from peakrdl_uvm import UVMExporter
 import argparse
 
+from systemrdl import RDLCompiler, RDLCompileError
+# from peakrdl.verilog import VerilogExporter
+
+try:
+    # newer version
+    from peakrdl_ipxact import IPXACTExporter
+    from peakrdl_uvm import UVMExporter
+except:
+    # older version
+    from peakrdl.ipxact import IPXACTExporter
+    from peakrdl.uvm import UVMExporter
+
 def cli(args):
     parser = argparse.ArgumentParser(description='rdl2any')
     # register format options
     parser.add_argument("-f", "--fname", help="register file description .rdl", action='store', type = str, default="./devices/rdl/basic.rdl")
     parser.add_argument("-ofmt", "--out-format", help="output format", action='store', type = str, default="ipxact", choices=["ipxact","uvm"])
 
     return parser.parse_args(args)
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie/tools/rdl2verilog.py` & `cheap_pie-0.1.17/src/cheap_pie/tools/rdl2verilog.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/tools/reload_module.py` & `cheap_pie-0.1.17/src/cheap_pie/tools/reload_module.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/tools/search.py` & `cheap_pie-0.1.17/src/cheap_pie/tools/search.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/tools/test_rdl.py` & `cheap_pie-0.1.17/src/cheap_pie/tools/test_rdl.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-0.1.17/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-0.1.17/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-0.1.17/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.16/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files 15% similar despite different names*

```diff
@@ -128,18 +128,42 @@
 
         self.sim.io.valid = 0
         self.sim.clock.tick()
 
         # print(hex(outval))
         return outval
 
+def verilator_version():
+    import subprocess
+    result = subprocess.run(['verilator', '--version'], stdout=subprocess.PIPE)
+    ver = result.stdout.split()[1]
+    return ver.decode("utf-8") 
+
+def verilator_version_ok():
+    # check Verilated::flushCall() exist
+    # https://github.com/chipsalliance/chisel3/issues/1565
+    from packaging import version
+    ver = verilator_version()
+    # print(ver)
+    if ( version.parse(ver) < version.parse("4.036") or
+         version.parse(ver) > version.parse("4.102")):
+        return True
+    else:
+        return False
+
 def test_cp_pyverilator(args = []):
-    p = cli()
-    hif = cp_pyverilator_transport(p.fname)
-    
-    val = literal_eval('0x5A5A5A5A')
-    hif.hifwrite(val = val)
-    print( hex(hif.hifread()) )
-    assert( hif.hifread() == val )
+
+    if verilator_version_ok():
+        p = cli(args)
+        hif = cp_pyverilator_transport(p.fname)
+        
+        val = literal_eval('0x5A5A5A5A')
+        hif.hifwrite(val = val)
+        print( hex(hif.hifread()) )
+        assert( hif.hifread() == val )
+
+    else:
+        print('Warning: pyverilator not working anymore with verilator versions between 4.036 and 4.102.')
+        print('https://github.com/chipsalliance/chisel3/issues/1565')
 
 if __name__ == '__main__':
     test_cp_pyverilator(sys.argv[1:])
```

### Comparing `cheap_pie-0.1.16/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-0.1.17/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

