# Comparing `tmp/pretix-mpesa-mz-1.0.1.tar.gz` & `tmp/pretix-mpesa-mz-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.0.1.tar", last modified: Fri May  5 16:56:30 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.0.2.tar", last modified: Fri May  5 17:11:22 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.0.1.tar` & `pretix-mpesa-mz-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.257906 pretix-mpesa-mz-1.0.1/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1686 2023-05-05 16:56:30.258906 pretix-mpesa-mz-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.142912 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1686 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.177909 pretix-mpesa-mz-1.0.1/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-05-05 16:18:47.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.074915 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.073911 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.187909 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.192909 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.204912 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     8467 2023-05-05 16:46:27.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.079911 pretix-mpesa-mz-1.0.1/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.210914 pretix-mpesa-mz-1.0.1/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.083911 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.244912 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      280 2023-05-03 13:51:46.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      184 2023-04-27 15:38:33.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      903 2023-05-05 16:56:30.262918 pretix-mpesa-mz-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.253907 pretix-mpesa-mz-1.0.1/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.584766 pretix-mpesa-mz-1.0.2/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1686 2023-05-05 17:11:22.585764 pretix-mpesa-mz-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.484674 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1686 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-05-05 17:11:22.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.508670 pretix-mpesa-mz-1.0.2/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-05-05 17:08:46.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.422666 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.420665 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.519626 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.524628 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.533792 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     8589 2023-05-05 17:09:40.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.427666 pretix-mpesa-mz-1.0.2/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.540773 pretix-mpesa-mz-1.0.2/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.429666 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.573764 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      280 2023-05-03 13:51:46.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      184 2023-04-27 15:38:33.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      903 2023-05-05 17:11:22.587768 pretix-mpesa-mz-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.579764 pretix-mpesa-mz-1.0.2/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.0.1/LICENSE` & `pretix-mpesa-mz-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/PKG-INFO` & `pretix-mpesa-mz-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.0.1
+Version: 1.0.2
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.0.1/README.rst` & `pretix-mpesa-mz-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.0.1
+Version: 1.0.2
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.0.2/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.0.2/pretix_mpesamz/payment.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,16 +109,17 @@
     @property
     def payment_form_fields(self):
         # Validate: ensure only valid numbers can be entered
         msisdn_field = ('msisdn',
             forms.IntegerField(
             label='Número (+258):',
             required=True,
-           min_value=840000000,
-           max_value=859999999
+            min_value=840000000,
+            max_value=859999999,
+            error_messages={'invalid':'Por favor, introduza um número 84 ou 85 válido'}
         ))
         return OrderedDict([
             msisdn_field,
         ])
     
     def payment_form_render(self, request):
         form = self.payment_form(request)
@@ -211,15 +212,15 @@
     ########################################################
     #                   Called to display Order 
     #                   info in Control Panel
     ########################################################
     def payment_control_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/control.html')
 
-        if 'conversation' in payment.info:
+        if payment.info is not None or 'conversation' in payment.info:
             payment_info = json.loads(payment.info)
         else:
             return _("Pagamento via M-Pesa sem sucesso.")
         
         ctx = {
             'conversationID': payment_info['conversation'],
             'msisdn': payment_info['msisdn'],
```

### Comparing `pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/setup.cfg` & `pretix-mpesa-mz-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.1/setup.py` & `pretix-mpesa-mz-1.0.2/setup.py`

 * *Files identical despite different names*

