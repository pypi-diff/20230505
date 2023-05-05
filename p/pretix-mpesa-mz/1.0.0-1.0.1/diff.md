# Comparing `tmp/pretix-mpesa-mz-1.0.0.tar.gz` & `tmp/pretix-mpesa-mz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.0.0.tar", last modified: Wed May  3 17:04:11 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.0.1.tar", last modified: Fri May  5 16:56:30 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.0.0.tar` & `pretix-mpesa-mz-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.514165 pretix-mpesa-mz-1.0.0/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1686 2023-05-03 17:04:11.515162 pretix-mpesa-mz-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.411160 pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1686 2023-05-03 17:04:10.000000 pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-05-03 17:04:11.000000 pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:04:10.000000 pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-03 17:04:10.000000 pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 17:04:10.000000 pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.435161 pretix-mpesa-mz-1.0.0/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.344159 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.342160 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.446161 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.452172 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.463164 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     8398 2023-05-03 15:01:00.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.349164 pretix-mpesa-mz-1.0.0/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.469164 pretix-mpesa-mz-1.0.0/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.352160 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.505163 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      280 2023-05-03 13:51:46.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      184 2023-04-27 15:38:33.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      903 2023-05-03 17:04:11.518161 pretix-mpesa-mz-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:04:11.509161 pretix-mpesa-mz-1.0.0/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.257906 pretix-mpesa-mz-1.0.1/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1686 2023-05-05 16:56:30.258906 pretix-mpesa-mz-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.142912 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1686 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-05 16:56:29.000000 pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.177909 pretix-mpesa-mz-1.0.1/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-05-05 16:18:47.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.074915 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.073911 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.187909 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.192909 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.204912 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     8467 2023-05-05 16:46:27.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.079911 pretix-mpesa-mz-1.0.1/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.210914 pretix-mpesa-mz-1.0.1/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.083911 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.244912 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      280 2023-05-03 13:51:46.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      184 2023-04-27 15:38:33.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      903 2023-05-05 16:56:30.262918 pretix-mpesa-mz-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:56:30.253907 pretix-mpesa-mz-1.0.1/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.1/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.0.0/LICENSE` & `pretix-mpesa-mz-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/PKG-INFO` & `pretix-mpesa-mz-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.0.0
+Version: 1.0.1
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.0.0/README.rst` & `pretix-mpesa-mz-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.0.0
+Version: 1.0.1
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.0.0/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.0.1/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.0.1/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.0.1/pretix_mpesamz/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,19 @@
     ########################################################
     #                   General Settings
     ########################################################
     @property
     def payment_form_fields(self):
         # Validate: ensure only valid numbers can be entered
         msisdn_field = ('msisdn',
-            forms.CharField(
-            label='Número 84/85',
+            forms.IntegerField(
+            label='Número (+258):',
             required=True,
-            max_length=9
+           min_value=840000000,
+           max_value=859999999
         ))
         return OrderedDict([
             msisdn_field,
         ])
     
     def payment_form_render(self, request):
         form = self.payment_form(request)
@@ -148,15 +149,15 @@
 
         
     def execute_payment(self, request, payment):
         msisdn = request.session.get('payment_%s_msisdn' % self.identifier, '')
 
         try:
             payment_data = {
-                'from': "258" + msisdn,   
+                'from': "258" + str(msisdn),   
                 'reference': payment.order.code,      
                 'transaction': 'TEST' + str(randint(0, 1000)), 
                 'amount': str(int(float(payment.amount)))
             }
 
             result = self.execute_mpesa_payment(payment_data)
 
@@ -209,18 +210,19 @@
 
     ########################################################
     #                   Called to display Order 
     #                   info in Control Panel
     ########################################################
     def payment_control_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/control.html')
-        if payment.info:
+
+        if 'conversation' in payment.info:
             payment_info = json.loads(payment.info)
         else:
-            return _("No payment information available.")
+            return _("Pagamento via M-Pesa sem sucesso.")
         
         ctx = {
             'conversationID': payment_info['conversation'],
             'msisdn': payment_info['msisdn'],
             'description': payment_info['description'],
         }
         return template.render(ctx)
```

### Comparing `pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.0.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/setup.cfg` & `pretix-mpesa-mz-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.0/setup.py` & `pretix-mpesa-mz-1.0.1/setup.py`

 * *Files identical despite different names*

