# Comparing `tmp/ms_mailbox_reader-0.1.3.tar.gz` & `tmp/ms_mailbox_reader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_mailbox_reader-0.1.3.tar", last modified: Fri May  5 21:28:40 2023, max compression
+gzip compressed data, was "ms_mailbox_reader-1.0.0.tar", last modified: Fri May  5 21:41:25 2023, max compression
```

## Comparing `ms_mailbox_reader-0.1.3.tar` & `ms_mailbox_reader-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:40.811537 ms_mailbox_reader-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-05 21:28:31.000000 ms_mailbox_reader-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:28:40.811537 ms_mailbox_reader-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 21:28:31.000000 ms_mailbox_reader-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:40.811537 ms_mailbox_reader-0.1.3/ms_mailbox_reader/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 21:28:31.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-05 21:28:31.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:40.811537 ms_mailbox_reader-0.1.3/ms_mailbox_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:28:40.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 21:28:40.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:28:40.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 21:28:40.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 21:28:40.000000 ms_mailbox_reader-0.1.3/ms_mailbox_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:28:40.811537 ms_mailbox_reader-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 21:28:31.000000 ms_mailbox_reader-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:41:25.677637 ms_mailbox_reader-1.0.0/ms_mailbox_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 21:41:25.000000 ms_mailbox_reader-1.0.0/ms_mailbox_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:41:25.681637 ms_mailbox_reader-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 21:41:12.000000 ms_mailbox_reader-1.0.0/setup.py
```

### Comparing `ms_mailbox_reader-0.1.3/LICENSE` & `ms_mailbox_reader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_mailbox_reader-0.1.3/README.md` & `ms_mailbox_reader-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 # ms-mailbox-reader
-A python package for windows which allows easy readnig of email 
-messages from a local mailbox. Tested with Outlook and Microsoft Exchange. 
+A python package for windows which allows easy reading of email 
+messages from a local mailbox. Tested with Outlook + Microsoft Exchange on a Windows 11 PC. 
 
 
 ### Basic Usage
 ```python
 from ms_mailbox_reader.client import MsExchangeClient, MessageFilter
 
-msClient = MsExchangeClient()
+# Create the message reader
+message_reader = MsOutlookMessageReader()
+
+# Timedelta representing the last two hours
 last_n_hours = datetime.now() - timedelta(hours=2)
+
+# Create a filter to limit returned messages to a max of 25, 
+# those which were sent from @mydomain.com and 
+# received in the last two hours
 filter_params = MessageFilter(sender_email="@mydomain.com",
                               received_since = last_n_hours,
                               limit=25)
 
-messages = msClient.get_outlook_messages(filter_params)
+# Get the message list
+messages = message_reader.get_outlook_messages(filter_params)
 
+# Do stuff with the messages
 for message in messages:
     print(message.sender_name)
     print(message.body)
     print("=====================")
 ```
```

### Comparing `ms_mailbox_reader-0.1.3/ms_mailbox_reader/client.py` & `ms_mailbox_reader-1.0.0/ms_mailbox_reader/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.sender_name = sender_name
         self.subject = subject.strip()
         self.date = date
         self.body = body.strip()
         self.conversation_id = None
 
 
-class MsExchangeClient:
+class MsOutlookMessageReader:
     @staticmethod
     def __extract_content_before_from_pattern(message_body: str) -> str:
         """
         Extracts the latest unique message from a message body by removing all
         previous responses and duplicated message history.
 
         Args:
@@ -134,15 +134,15 @@
 
         outlook = win32com.client.Dispatch(
             "Outlook.Application").GetNamespace("MAPI")
 
         # Get the default Inbox folder
         inbox = outlook.GetDefaultFolder(6)  # 6 represents the Inbox folder
 
-        message_filter = message_filter or MsExchangeClient.__get_default_message_filter()
+        message_filter = message_filter or MsOutlookMessageReader.__get_default_message_filter()
 
         # Get all messages that match the filter
         messages = inbox.Items.Restrict(message_filter.render())
         messages.Sort("[ReceivedTime]", True)
 
         message_counter = 0
         for message in messages:
@@ -154,13 +154,13 @@
 
             if message_filter.sender_email and message_filter.sender_email not in sender_email:
                 continue
 
             if message_filter.subject and message_filter.subject not in subject:
                 continue
 
-            original_message_content = MsExchangeClient.__extract_content_before_from_pattern(
+            original_message_content = MsOutlookMessageReader.__extract_content_before_from_pattern(
                 message.Body)
 
             yield SimpleMessage(message.SenderName, subject, message.ReceivedTime, original_message_content)
 
             message_counter += 1
```

