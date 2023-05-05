# Comparing `tmp/django-mailing-0.1beta9.tar.gz` & `tmp/django-mailing-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mailing-0.1beta9.tar", last modified: Thu Jan 17 15:51:28 2013, max compression
+gzip compressed data, was "dist/django-mailing-0.2.tar", last modified: Fri May  5 16:23:21 2023, max compression
```

## Comparing `django-mailing-0.1beta9.tar` & `django-mailing-0.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)       41 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/CHANGES.txt
-drwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/mailing/
-drwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/mailing/templates/
-drwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/mailing/templates/mailing/
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     3245 2013-01-11 16:28:53.000000 django-mailing-0.1beta9/mailing/templates/mailing/base.html
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)      150 2013-01-11 16:28:53.000000 django-mailing-0.1beta9/mailing/templates/mailing/base.txt
-drwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/
--rw-rw-r--   0 ampadmin  (1000) ampadmin  (1000)    12246 2013-01-11 16:28:53.000000 django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/email.html
--rw-rw-r--   0 ampadmin  (1000) ampadmin  (1000)     2555 2013-01-11 16:28:53.000000 django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/README.markdown
--rw-rw-r--   0 ampadmin  (1000) ampadmin  (1000)     6542 2013-01-11 16:28:53.000000 django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/email_lite.html
--rw-rw-r--   0 ampadmin  (1000) ampadmin  (1000)      352 2013-01-11 16:28:53.000000 django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/contributors.txt
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/mailing/models.py
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)      477 2013-01-17 15:48:45.000000 django-mailing-0.1beta9/mailing/__init__.py
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     4010 2013-01-17 15:48:45.000000 django-mailing-0.1beta9/mailing/mail.py
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)       26 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/mailing/views.py
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     2120 2013-01-17 15:48:45.000000 django-mailing-0.1beta9/mailing/shortcuts.py
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     1641 2013-01-11 17:46:58.000000 django-mailing-0.1beta9/mailing/tasks.py
-drwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)        0 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/docs/
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     8415 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/docs/usage.txt
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     1113 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/LICENSE.txt
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)      178 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/AUTHORS.txt
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     8415 2013-01-11 16:23:25.000000 django-mailing-0.1beta9/README.txt
--rwxrwxr-x   0 ampadmin  (1000) ampadmin  (1000)     1099 2013-01-11 17:46:58.000000 django-mailing-0.1beta9/setup.py
--rw-rw-r--   0 ampadmin  (1000) ampadmin  (1000)    10899 2013-01-17 15:51:28.000000 django-mailing-0.1beta9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:23:21.000000 django-mailing-0.2/
+-rwxr-xr-x   0 root         (0) root         (0)      178 2023-05-05 14:19:38.000000 django-mailing-0.2/AUTHORS.txt
+-rwxr-xr-x   0 root         (0) root         (0)       41 2023-05-05 14:19:38.000000 django-mailing-0.2/CHANGES.txt
+-rwxr-xr-x   0 root         (0) root         (0)     1113 2023-05-05 14:19:38.000000 django-mailing-0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    10894 2023-05-05 16:23:21.000000 django-mailing-0.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     8415 2023-05-05 14:19:38.000000 django-mailing-0.2/README.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:23:21.000000 django-mailing-0.2/docs/
+-rwxr-xr-x   0 root         (0) root         (0)     8415 2023-05-05 14:19:38.000000 django-mailing-0.2/docs/usage.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:23:21.000000 django-mailing-0.2/mailing/
+-rwxr-xr-x   0 root         (0) root         (0)      525 2023-05-05 14:22:36.000000 django-mailing-0.2/mailing/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5030 2023-05-05 15:32:40.000000 django-mailing-0.2/mailing/mail.py
+-rwxr-xr-x   0 root         (0) root         (0)     5077 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/mail.py.bak
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/models.py
+-rwxr-xr-x   0 root         (0) root         (0)     2263 2023-05-05 15:32:40.000000 django-mailing-0.2/mailing/shortcuts.py
+-rwxr-xr-x   0 root         (0) root         (0)     2265 2023-05-05 14:36:26.000000 django-mailing-0.2/mailing/shortcuts.py.bak
+-rwxr-xr-x   0 root         (0) root         (0)     1865 2023-05-05 15:45:35.000000 django-mailing-0.2/mailing/tasks.py
+-rwxr-xr-x   0 root         (0) root         (0)     1880 2023-05-05 14:26:22.000000 django-mailing-0.2/mailing/tasks.py.bak
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:23:21.000000 django-mailing-0.2/mailing/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:23:21.000000 django-mailing-0.2/mailing/templates/mailing/
+-rwxr-xr-x   0 root         (0) root         (0)     3245 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/templates/mailing/base.html
+-rwxr-xr-x   0 root         (0) root         (0)      150 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/templates/mailing/base.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:23:21.000000 django-mailing-0.2/mailing/templates/mailing/email_boiletplate/
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/templates/mailing/email_boiletplate/README.markdown
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/templates/mailing/email_boiletplate/contributors.txt
+-rw-r--r--   0 root         (0) root         (0)    12246 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/templates/mailing/email_boiletplate/email.html
+-rw-r--r--   0 root         (0) root         (0)     6542 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/templates/mailing/email_boiletplate/email_lite.html
+-rwxr-xr-x   0 root         (0) root         (0)       26 2023-05-05 14:19:38.000000 django-mailing-0.2/mailing/views.py
+-rwxr-xr-x   0 root         (0) root         (0)     1099 2023-05-05 14:19:38.000000 django-mailing-0.2/setup.py
```

### Comparing `django-mailing-0.1beta9/mailing/templates/mailing/base.html` & `django-mailing-0.2/mailing/templates/mailing/base.html`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/email.html` & `django-mailing-0.2/mailing/templates/mailing/email_boiletplate/email.html`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/README.markdown` & `django-mailing-0.2/mailing/templates/mailing/email_boiletplate/README.markdown`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/mailing/templates/mailing/email_boiletplate/email_lite.html` & `django-mailing-0.2/mailing/templates/mailing/email_boiletplate/email_lite.html`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/mailing/mail.py` & `django-mailing-0.2/mailing/mail.py.bak`

 * *Files 15% similar despite different names*

```diff
@@ -16,46 +16,60 @@
         self.value = value
     def __str__(self):
         return repr(self.value if value else '')
 
 def send_email_default(*args, **kwargs):
     send_email(args[3],args[0],args[1], from_email=args[2], category='django core email')
 
-def send_email(recipients, subject, text_content=None, html_content=None, from_email=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False):
+def send_email(recipients, subject, text_content=None, html_content=None, from_email=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None):
     """
     Will send a multi-format email to recipients. Email may be queued through celery
     """
     from django.conf import settings
     if not bypass_queue and hasattr(settings, 'MAILING_USE_CELERY') and settings.MAILING_USE_CELERY:
         from celery.execute import send_task
-        return send_task('mailing.queue_send_email',[recipients, subject, text_content, html_content, from_email, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers])
+        return send_task('mailing.queue_send_email',[recipients, subject, text_content, html_content, from_email, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files])
     else:
 
+        header_category_value = '%s%s' % (settings.MAILING_HEADER_CATEGORY_PREFIX if hasattr(settings, 'MAILING_HEADER_CATEGORY_PREFIX') else '', category)
         # Check for sendgrid support and add category header
         # --------------------------------
         if hasattr(settings, 'MAILING_USE_SENDGRID'):
             send_grid_support = settings.MAILING_USE_SENDGRID
         else:
             send_grid_support = False
 
         if not headers:
             headers = dict()        
         if send_grid_support and category:
-            headers['X-SMTPAPI'] = '{"category": "%s%s"}' % (settings.MAILING_SENDGRID_CATEGORY_PREFIX if hasattr(settings, 'MAILING_SENDGRID_CATEGORY_PREFIX') else '', category)
+            headers['X-SMTPAPI'] = '{"category": "%s"}' % header_category_value
+
+        # Check for Mailgun support and add label header
+        # --------------------------------
+        if hasattr(settings, 'MAILING_USE_MAILGUN'):
+            mailgun_support = settings.MAILING_USE_MAILGUN
+        else:
+            mailgun_support = False
+
+        if not headers:
+            headers = dict()        
+        if mailgun_support and category:
+            headers['X-Mailgun-Tag'] = header_category_value
+
 
         # Ensure recipients are in a list
         # --------------------------------
         if isinstance(recipients, basestring):
             recipients_list = [recipients]
         else:
             recipients_list = recipients
 
         # Check if we need to hijack the email
         # --------------------------------
-        if hasattr(settings, 'MAILING_MAILTO_HIJACK'):
+        if hasattr(settings, 'MAILING_MAILTO_HIJACK') and not bypass_hijacking:
             headers['X-MAILER-ORIGINAL-MAILTO'] = ','.join(recipients_list)
             recipients_list = [settings.MAILING_MAILTO_HIJACK]
 
         if not subject:
             raise MailerMissingSubjectError('Subject not supplied')
 
         # Send ascii, html or multi-part email
@@ -68,10 +82,22 @@
                 html_content = render_to_string('mailing/base.html', {'mailing_html_body': html_content, 'mailing_subject': subject, 'settings': settings}) if html_content else None
                 translation.activate(prev_language)
             msg = EmailMultiAlternatives(subject, text_content if text_content else html_content, from_email if from_email else settings.DEFAULT_FROM_EMAIL, recipients_list, cc=cc, bcc=bcc, attachments=attachments, headers = headers)
             if html_content and text_content:
                 msg.attach_alternative(html_content, "text/html")
             elif html_content: # Only HTML
                 msg.content_subtype = "html"
+
+            # Attach files through attach_files helper
+            # --------------------------------
+            if attach_files:
+                for att in attach_files:  # attachments are tuples of (filepath, mimetype, filename)
+                    with open(att[0], 'rb') as f:
+                        content = f.read()
+                    msg.attach(att[2], content, att[1])
+
+            # Send email
+            # --------------------------------
+
             msg.send(fail_silently=fail_silently)
         else:
             raise MailerInvalidBodyError('No text or html body supplied.')
```

### Comparing `django-mailing-0.1beta9/mailing/shortcuts.py` & `django-mailing-0.2/mailing/shortcuts.py.bak`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.conf import settings
 from django.template.loader import render_to_string
 from django.template import TemplateDoesNotExist
 from django.utils import translation
 
-from mail import send_email
+from mailing.mail import send_email
 
-def render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False):
+def render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_queue=False, bypass_hijacking=False, attach_files=None):
     if not bypass_queue and hasattr(settings, 'MAILING_USE_CELERY') and settings.MAILING_USE_CELERY:
         from celery.execute import send_task
-        return send_task('mailing.queue_render_send_email',[recipients, template, data, from_email, subject, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers])
+        return send_task('mailing.queue_render_send_email',[recipients, template, data, from_email, subject, use_base_template, category, fail_silently, language if language else translation.get_language(), cc, bcc, attachments, headers, bypass_hijacking, attach_files])
     else:
         # Set language
         # --------------------------------
         prev_language = translation.get_language()
         language and translation.activate(language)
         if subject:
             my_subject = subject
@@ -34,9 +34,9 @@
 
         try:
             html_content = render_to_string('%s.html' % template, data)
         except TemplateDoesNotExist:
             html_content = None
 
         translation.activate(prev_language)
-        send_email(recipients, my_subject, text_content, html_content, from_email, use_base_template, category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True)
+        send_email(recipients, my_subject, text_content, html_content, from_email, use_base_template, category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files)
```

### Comparing `django-mailing-0.1beta9/mailing/tasks.py` & `django-mailing-0.2/mailing/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from django.conf import settings
-
-from celery.task import task
-
-from mail import send_email
-from shortcuts import render_send_email
-
-@task(name="mailing.queue_send_email")
-def queue_send_email(recipients, subject, text_content=None, html_content=None, from_email=settings.DEFAULT_FROM_EMAIL, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None): 
-    
-    logger = queue_send_email.get_logger()
-    logger.debug('Sending %s to %s' % (subject, ','.join(recipients), ))
-
-    send_email(recipients=recipients, subject=subject, text_content=text_content, html_content=html_content, from_email=from_email, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True)
-
-    return True
-
-@task(name="mailing.queue_render_send_email")
-def queue_render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None):
-    
-    logger = queue_render_send_email.get_logger()
-
-    logger.debug('Rendering and sending %s to %s' % (template, ','.join(recipients), ))
-
-    render_send_email(recipients=recipients, template=template, data=data, from_email=from_email, subject=subject, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True)
-
-    return True
+from __future__ import absolute_import
+from django.conf import settings
+
+from celery.task import task
+
+from .mail import send_email
+from .shortcuts import render_send_email
+
+@task(name="mailing.queue_send_email")
+def queue_send_email(recipients, subject, text_content=None, html_content=None, from_email=settings.DEFAULT_FROM_EMAIL, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None): 
+    
+    logger = queue_send_email.get_logger()
+    logger.debug('Sending %s to %s' % (subject, ','.join(recipients), ))
+
+    send_email(recipients=recipients, subject=subject, text_content=text_content, html_content=html_content, from_email=from_email, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files)
+
+    return True
+
+@task(name="mailing.queue_render_send_email")
+def queue_render_send_email(recipients, template, data, from_email=settings.DEFAULT_FROM_EMAIL, subject=None, use_base_template=True, category=None, fail_silently=False, language=None, cc=None, bcc=None, attachments=None, headers=None, bypass_hijacking=False, attach_files=None):
+    
+    logger = queue_render_send_email.get_logger()
+
+    logger.debug('Rendering and sending %s to %s' % (template, ','.join(recipients), ))
+
+    render_send_email(recipients=recipients, template=template, data=data, from_email=from_email, subject=subject, use_base_template=use_base_template, category=category, fail_silently=fail_silently, language=language, cc=cc, bcc=bcc, attachments=attachments, headers=headers, bypass_queue=True, bypass_hijacking=bypass_hijacking, attach_files=attach_files)
+
+    return True
```

### Comparing `django-mailing-0.1beta9/docs/usage.txt` & `django-mailing-0.2/README.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/LICENSE.txt` & `django-mailing-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/README.txt` & `django-mailing-0.2/docs/usage.txt`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/setup.py` & `django-mailing-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-mailing-0.1beta9/PKG-INFO` & `django-mailing-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mailing
-Version: 0.1beta9
+Version: 0.2
 Summary: A flexible Django app for templated mailings with support for celery queuing, SendGrid and more.
 Home-page: http://github.com/JeromeParadis/django-mailing
 Author: Jerome Paradis
 Author-email: jparadis@paradivision.com
 License: LICENSE.txt
 Description: 
         =====
```

