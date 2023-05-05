# Comparing `tmp/for-django-projects-1.0.3.tar.gz` & `tmp/for-django-projects-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "for-django-projects-1.0.3.tar", last modified: Thu May  4 17:23:47 2023, max compression
+gzip compressed data, was "for-django-projects-1.0.4.tar", last modified: Thu May  4 18:03:02 2023, max compression
```

## Comparing `for-django-projects-1.0.3.tar` & `for-django-projects-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.169842 for-django-projects-1.0.3/
--rw-rw-rw-   0        0        0     1010 2023-05-04 17:23:47.169842 for-django-projects-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-05-04 17:16:18.000000 for-django-projects-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.127312 for-django-projects-1.0.3/for_django_projects/
--rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.3/for_django_projects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.150369 for-django-projects-1.0.3/for_django_projects/alertas/
--rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.3/for_django_projects/alertas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.157685 for-django-projects-1.0.3/for_django_projects/form_utils/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/__init__.py
--rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/admin.py
--rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/fields.py
--rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/forms.py
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/models.py
--rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.159646 for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/
--rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/form_utils.py
--rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/utils.py
--rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/form_utils/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.162648 for-django-projects-1.0.3/for_django_projects/pwa/
--rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/__init__.py
--rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/app_settings.py
--rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.163653 for-django-projects-1.0.3/for_django_projects/pwa/templatetags/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/templatetags/__init__.py
--rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/templatetags/pwa.py
--rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/urls.py
--rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.3/for_django_projects/pwa/views.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.168841 for-django-projects-1.0.3/for_django_projects/utils/
--rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.3/for_django_projects/utils/__init__.py
--rw-rw-rw-   0        0        0    24113 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/custom_models.py
--rw-rw-rw-   0        0        0     3012 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/decoradores.py
--rw-rw-rw-   0        0        0    18629 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/funciones.py
--rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.3/for_django_projects/utils/funciones_adicionales.py
--rw-rw-rw-   0        0        0     3137 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/for_django_projects/utils/models_utils.py
--rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.3/for_django_projects/utils/validadores.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:23:47.149357 for-django-projects-1.0.3/for_django_projects.egg-info/
--rw-rw-rw-   0        0        0     1010 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-04 17:23:47.000000 for-django-projects-1.0.3/for_django_projects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 17:23:47.169842 for-django-projects-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-05-04 17:23:25.000000 for-django-projects-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.674652 for-django-projects-1.0.4/
+-rw-rw-rw-   0        0        0     1195 2023-05-04 18:03:02.673621 for-django-projects-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-05-04 18:02:34.000000 for-django-projects-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.640493 for-django-projects-1.0.4/for_django_projects/
+-rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.4/for_django_projects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.655334 for-django-projects-1.0.4/for_django_projects/alertas/
+-rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.4/for_django_projects/alertas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.661336 for-django-projects-1.0.4/for_django_projects/form_utils/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/__init__.py
+-rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/admin.py
+-rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/fields.py
+-rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/forms.py
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/models.py
+-rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.663437 for-django-projects-1.0.4/for_django_projects/form_utils/templatetags/
+-rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/templatetags/form_utils.py
+-rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/utils.py
+-rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/form_utils/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.666481 for-django-projects-1.0.4/for_django_projects/pwa/
+-rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/__init__.py
+-rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/app_settings.py
+-rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.667485 for-django-projects-1.0.4/for_django_projects/pwa/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/templatetags/pwa.py
+-rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/urls.py
+-rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.4/for_django_projects/pwa/views.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.673481 for-django-projects-1.0.4/for_django_projects/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.4/for_django_projects/utils/__init__.py
+-rw-rw-rw-   0        0        0    24187 2023-05-04 17:54:34.000000 for-django-projects-1.0.4/for_django_projects/utils/custom_models.py
+-rw-rw-rw-   0        0        0     3071 2023-05-04 18:02:08.000000 for-django-projects-1.0.4/for_django_projects/utils/decoradores.py
+-rw-rw-rw-   0        0        0    18629 2023-05-04 17:23:25.000000 for-django-projects-1.0.4/for_django_projects/utils/funciones.py
+-rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.4/for_django_projects/utils/funciones_adicionales.py
+-rw-rw-rw-   0        0        0     3137 2023-05-04 17:23:25.000000 for-django-projects-1.0.4/for_django_projects/utils/models_utils.py
+-rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.4/for_django_projects/utils/validadores.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:03:02.654338 for-django-projects-1.0.4/for_django_projects.egg-info/
+-rw-rw-rw-   0        0        0     1195 2023-05-04 18:03:02.000000 for-django-projects-1.0.4/for_django_projects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-05-04 18:03:02.000000 for-django-projects-1.0.4/for_django_projects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 18:03:02.000000 for-django-projects-1.0.4/for_django_projects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-04 18:03:02.000000 for-django-projects-1.0.4/for_django_projects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-04 18:03:02.000000 for-django-projects-1.0.4/for_django_projects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 18:03:02.674652 for-django-projects-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      919 2023-05-04 18:02:56.000000 for-django-projects-1.0.4/setup.py
```

### Comparing `for-django-projects-1.0.3/PKG-INFO` & `for-django-projects-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: for-django-projects
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package of libraries for Django projects
 Home-page: https://github.com/jasmanysanchez/for-django-projects
 Author: Jasmany Sanchez Mendez
 Author-email: jasmanysanchez97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,12 +27,20 @@
     ...
     'for_django_projects.form_utils',
     'for_django_projects.pwa'
     ...
 ]
 ```
 
+Add in settings.py:
+
+```sh
+SIMBOLO_MONEDA = '$'
+URL_GENERAL = 'http://your_domain.com'
+CONSTRAINT_MSG = {} #dict of name of constraints as key and error message as value  
+```
+
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `for-django-projects-1.0.3/README.md` & `for-django-projects-1.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -14,12 +14,20 @@
     ...
     'for_django_projects.form_utils',
     'for_django_projects.pwa'
     ...
 ]
 ```
 
+Add in settings.py:
+
+```sh
+SIMBOLO_MONEDA = '$'
+URL_GENERAL = 'http://your_domain.com'
+CONSTRAINT_MSG = {} #dict of name of constraints as key and error message as value  
+```
+
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `for-django-projects-1.0.3/for_django_projects/alertas/__init__.py` & `for-django-projects-1.0.4/for_django_projects/alertas/__init__.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/form_utils/fields.py` & `for-django-projects-1.0.4/for_django_projects/form_utils/fields.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/form_utils/forms.py` & `for-django-projects-1.0.4/for_django_projects/form_utils/forms.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/form_utils/templatetags/form_utils.py` & `for-django-projects-1.0.4/for_django_projects/form_utils/templatetags/form_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/form_utils/utils.py` & `for-django-projects-1.0.4/for_django_projects/form_utils/utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/form_utils/widgets.py` & `for-django-projects-1.0.4/for_django_projects/form_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/pwa/app_settings.py` & `for-django-projects-1.0.4/for_django_projects/pwa/app_settings.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/pwa/templatetags/pwa.py` & `for-django-projects-1.0.4/for_django_projects/pwa/templatetags/pwa.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/pwa/views.py` & `for-django-projects-1.0.4/for_django_projects/pwa/views.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/utils/custom_models.py` & `for-django-projects-1.0.4/for_django_projects/utils/custom_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 def build_json_data(self) -> str:
     from django.http import JsonResponse
     return JsonResponse(self.build_dict_data()).content.decode()
 
 class NormalModel(models.Model):
 
     def __init__(self, *args, **kwargs):
+        SIMBOLO_MONEDA = getattr(settings, 'SIMBOLO_MONEDA', '$')
         from dateutil.tz import tz
         super().__init__(*args, **kwargs)
         for x in self._meta.fields:
             f = x.name
             if isinstance(self._meta.get_field(f), models.BooleanField):
                 is_true = customgetattr(self, f)
                 if is_true == None:
@@ -102,15 +103,15 @@
                 setattr(self, '%s_texthtml' % f, t)
                 t = "Sí" if is_true else "No"
                 setattr(self, '%s_yesorno' % f, t)
             if isinstance(self._meta.get_field(f), models.DecimalField):
                 t = customgetattr(self, f)
                 if t != None:
                     setattr(self, '%s_unlocalize' % f, str(t).replace(',', '.'))
-                    setattr(self, '%s_money' % f, "{}{}".format(settings.SIMBOLO_MONEDA, str(t).replace(',', '.')))
+                    setattr(self, '%s_money' % f, "{}{}".format(SIMBOLO_MONEDA, str(t).replace(',', '.')))
                     t = int(float(customgetattr(self, f)))
                     setattr(self, '%s_integer' % f, t)
             if isinstance(self._meta.get_field(f), models.DateTimeField):
                 t = customgetattr(self, f)
                 if t != None:
                     setattr(self, '%s_tz' % f, t.astimezone(tz.gettz(settings.TIME_ZONE)))
             if isinstance(self._meta.get_field(f), models.FileField):
@@ -143,15 +144,15 @@
                     setattr(self, '%s_extension' % f, extension)
 
                     setattr(self, '%s_fancybox' % f, create_function_fancybox('%s_fancybox_func' % f, **{
                         "archivo": file,
                         "archivo_is_image": is_image,
                         "archivo_extension": extension,
                         "icono": mark_safe(archivo_icon),
-                        "URL_GENERAL": settings.URL_GENERAL,
+                        "URL_GENERAL": getattr(settings, 'URL_GENERAL', ''),
                     }))
 
     def build_dict_data(self) -> dict:
         return build_dict_data(self)
 
     def build_json_data(self) -> str:
         return build_json_data(self)
```

### Comparing `for-django-projects-1.0.3/for_django_projects/utils/decoradores.py` & `for-django-projects-1.0.4/for_django_projects/utils/decoradores.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
                 val_func = JsonResponse(res_json, safe=False)
                 has_except = True
                 error_message = "Formulario no válido"
             except IntegrityError as ex:
                 has_except = True
                 msg = str(ex)
                 error_message = "Integrity Error"
-                for key in settings.CONSTRAINT_MSG_KEYS:
+                for key in getattr(settings, 'CONSTRAINT_MSG', {}).keys():
                     if re.search(f"\\b{key}\\b", msg):
-                        error_message = settings.CONSTRAINT_MSG[key]
+                        error_message = getattr(settings, 'CONSTRAINT_MSG', {}).get(key) or 'Integrity Error'
                 res_json.append(
                     {
                         'error': has_except,
                         "message": error_message
                     }
                 )
                 val_func = JsonResponse(res_json, safe=False)
```

### Comparing `for-django-projects-1.0.3/for_django_projects/utils/funciones.py` & `for-django-projects-1.0.4/for_django_projects/utils/funciones.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/utils/funciones_adicionales.py` & `for-django-projects-1.0.4/for_django_projects/utils/funciones_adicionales.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/utils/models_utils.py` & `for-django-projects-1.0.4/for_django_projects/utils/models_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects/utils/validadores.py` & `for-django-projects-1.0.4/for_django_projects/utils/validadores.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/for_django_projects.egg-info/PKG-INFO` & `for-django-projects-1.0.4/for_django_projects.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: for-django-projects
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package of libraries for Django projects
 Home-page: https://github.com/jasmanysanchez/for-django-projects
 Author: Jasmany Sanchez Mendez
 Author-email: jasmanysanchez97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,12 +27,20 @@
     ...
     'for_django_projects.form_utils',
     'for_django_projects.pwa'
     ...
 ]
 ```
 
+Add in settings.py:
+
+```sh
+SIMBOLO_MONEDA = '$'
+URL_GENERAL = 'http://your_domain.com'
+CONSTRAINT_MSG = {} #dict of name of constraints as key and error message as value  
+```
+
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `for-django-projects-1.0.3/for_django_projects.egg-info/SOURCES.txt` & `for-django-projects-1.0.4/for_django_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.3/setup.py` & `for-django-projects-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="for-django-projects",
-    version="1.0.3",
+    version="1.0.4",
     author="Jasmany Sanchez Mendez",
     author_email="jasmanysanchez97@gmail.com",
     description="Package of libraries for Django projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasmanysanchez/for-django-projects",
     packages=setuptools.find_packages(),
```

