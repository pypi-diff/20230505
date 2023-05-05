# Comparing `tmp/ntfy_wrapper-0.1.6.tar.gz` & `tmp/ntfy_wrapper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntfy_wrapper-0.1.6.tar", max compression
+gzip compressed data, was "ntfy_wrapper-0.1.7.tar", max compression
```

## Comparing `ntfy_wrapper-0.1.6.tar` & `ntfy_wrapper-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2022-11-09 22:16:23.728243 ntfy_wrapper-0.1.6/LICENSE
--rw-r--r--   0        0        0    13530 2022-11-15 15:17:28.955874 ntfy_wrapper-0.1.6/README.md
--rw-r--r--   0        0        0       45 2022-11-10 06:23:48.089088 ntfy_wrapper-0.1.6/ntfy_wrapper/__init__.py
--rw-r--r--   0        0        0    11311 2022-11-15 15:16:29.552862 ntfy_wrapper-0.1.6/ntfy_wrapper/cli.py
--rw-r--r--   0        0        0    16665 2022-11-14 16:21:15.331834 ntfy_wrapper-0.1.6/ntfy_wrapper/notifier.py
--rw-r--r--   0        0        0     5652 2022-11-11 18:23:29.995487 ntfy_wrapper-0.1.6/ntfy_wrapper/utils.py
--rw-r--r--   0        0        0      764 2022-11-15 15:17:12.051690 ntfy_wrapper-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    14652 1970-01-01 00:00:00.000000 ntfy_wrapper-0.1.6/setup.py
--rw-r--r--   0        0        0    14247 1970-01-01 00:00:00.000000 ntfy_wrapper-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-11-09 22:16:23.728243 ntfy_wrapper-0.1.7/LICENSE
+-rw-r--r--   0        0        0    13680 2023-05-05 17:50:59.759772 ntfy_wrapper-0.1.7/README.md
+-rw-r--r--   0        0        0      132 2023-05-05 17:50:59.760888 ntfy_wrapper-0.1.7/ntfy_wrapper/__init__.py
+-rw-r--r--   0        0        0    12918 2023-05-05 17:50:59.761659 ntfy_wrapper-0.1.7/ntfy_wrapper/cli.py
+-rw-r--r--   0        0        0    20485 2023-05-05 17:50:59.762985 ntfy_wrapper-0.1.7/ntfy_wrapper/notifier.py
+-rw-r--r--   0        0        0     6045 2023-05-05 17:50:59.763503 ntfy_wrapper-0.1.7/ntfy_wrapper/utils.py
+-rw-r--r--   0        0        0      764 2023-05-05 17:50:59.763832 ntfy_wrapper-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    14803 1970-01-01 00:00:00.000000 ntfy_wrapper-0.1.7/setup.py
+-rw-r--r--   0        0        0    14397 1970-01-01 00:00:00.000000 ntfy_wrapper-0.1.7/PKG-INFO
```

### Comparing `ntfy_wrapper-0.1.6/LICENSE` & `ntfy_wrapper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ntfy_wrapper-0.1.6/README.md` & `ntfy_wrapper-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <p align="center">
     <a href="https://github.com/vict0rsch/ntfy-wrapper" target="_blank">
         <img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/ntfy-txt.png">
     </a>
 </p>
 <p align="center">
-    <a href="https://pypi.org/project/ntfy-wrapper/"><img src="https://img.shields.io/badge/pypi%20package-0.1.6-yellowgreen" alt="PyPI version" height="18"></a>
+    <a href="https://pypi.org/project/ntfy-wrapper/"><img src="https://img.shields.io/badge/pypi%20package-0.1.7-yellowgreen" alt="PyPI version" height="18"></a>
     <a href="https://ntfy-wrapper.readthedocs.io/en/latest/index.html"><img src="https://img.shields.io/badge/docs-read%20the%20docs-blue" alt="PyPI version" height="18"></a>
     <a href="https://github.com/vict0rsch/ntfy-wrapper/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"><img src="https://img.shields.io/github/issues-raw/vict0rsch/ntfy-wrapper" alt="Open Issues" height="18"></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/codestyle-black-red" alt="Black code style" height="18"></a>
     <a href="https://github.com/vict0rsch/ntfy-wrapper/blob/main/LICENSE><img src="https://img.shields.io/github/license/vict0rsch/ntfy-wrapper" alt="License" height="18"></a>
 </p>
 
 `ntfy-wrapper` is a free and hassle-free customizable notifier for Python. No login, no API token, no fees, no bullshit.
@@ -115,23 +115,24 @@
 
 <a href="https://ntfy.sh/app"><img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/mermaid.png"></a>
 
 ## Configuration file
 
 `ntfy-wrapper` uses the INI standard along with `configparser` to parse the configuration file. It expects 2 sections:
 
-1. `[notifier_init]` with optional fields `emails = ` and `topics = ` to define systematic targets for the notification instead of putting them in your Python code
+1. `[notifier_init]` with optional fields `emails = `, `topics = ` and `base_url = ` to define systematic targets for the notification instead of putting them in your Python code. `base_url` allows to push to a different `ntfy` server than the default `https://ntfy.sh`.
 2. `[notify_defaults]` with optional fields listed below, which will define default parameters used by `Notifier.notify(...)`. For instance you can set default `title` and `tags` for your code's `.notify(...)` calls and override them at specific locations with keyword arguments `.notify(title="Non-default title")`
    1. The behavior of the `title`, `priority`, `tags`, `click`, `attach`, `actions` and `icon` keys is described in the [`ntfy` docs](https://ntfy.sh/docs/publish/)
 
 ```ini
 # For Notifier(emails=..., topics=...)
 [notifier_init]
 topics = my-secret-topic-1, mysecrettopic2
 emails = you@foo.bar
+base_url = https://custom-ntfy-instance.io
 
 # For Notifier.notify(title=..., priority=..., etc.)
 [notify_defaults]
 title = Message from ntfy-wrapper
 priority = 0
 tags = fire
 click =
```

### Comparing `ntfy_wrapper-0.1.6/ntfy_wrapper/cli.py` & `ntfy_wrapper-0.1.7/ntfy_wrapper/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -117,15 +117,35 @@
     if email not in emails:
         emails.append(email)
         conf["emails"] = emails
     else:
         print(f"email {email} already exists.")
         raise typer.Abort()
     write_conf(conf_path, conf)
-    print(f"🎉 Email {code(email)} added to {code(conf_path)}", style="green")
+
+
+@add_app.command("base_url")
+def add_base_url(url: str, conf_path: Optional[str] = None):
+    """
+    Adds an url to the config file to override the default https://ntfy.sh.
+    If --conf-path is not given, the current working directory will be used.
+    """
+    conf_path = get_conf_path(conf_path)
+    if not conf_path.exists():
+        raise typer.Abort(f"Config file not found at {str(conf_path)}")
+    conf = load_conf(conf_path)
+    base_url = conf.get("base_url", [])
+    if url not in base_url:
+        base_url.append(url)
+        conf["base_url"] = base_url
+    else:
+        print(f"base_url {url} already exists.")
+        raise typer.Abort()
+    write_conf(conf_path, conf)
+    print(f"🎉 URL {code(url)} added to {code(conf_path)}", style="green")
 
 
 @add_app.command("default")
 def add_default(key: str, value: str, conf_path: Optional[str] = None):
     """
     Adds a default to the config file.
     If --conf-path is not given, the current working directory will be used.
@@ -187,14 +207,34 @@
         conf["emails"] = emails
         write_conf(conf_path, conf)
         print(f"🎉 Email {code(email)} removed from {code(conf_path)}", style="green")
     else:
         print(f"Email {code(email)} does not exist. Ignoring.", style="yellow")
 
 
+@remove_app.command("base_url")
+def remove_base_url(url: str, conf_path: Optional[str] = None):
+    """
+    Removes an url from the config file.
+    If --conf-path is not given, the current working directory will be used.
+    """
+    conf_path = get_conf_path(conf_path)
+    if not conf_path.exists():
+        raise typer.BadParameter(f"Config file not found at {str(conf_path)}")
+    conf = load_conf(conf_path)
+    base_url = conf.get("base_url", "")
+    if url in base_url:
+        base_url = [u.strip() for u in base_url.split(",") if u.strip() != url.strip()]
+        conf["base_url"] = ", ".join(base_url)
+        write_conf(conf_path, conf)
+        print(f"🎉 URL {code(url)} removed from {code(conf_path)}", style="green")
+    else:
+        print(f"URL {code(url)} does not exist. Ignoring.", style="yellow")
+
+
 @remove_app.command("default")
 def remove_default(key: str, conf_path: Optional[str] = None):
     """
     Removes a default from the config file.
     If --conf-path is not given, the current working directory will be used.
     """
     conf_path = get_conf_path(conf_path)
@@ -312,24 +352,25 @@
 def describe(conf_path: Optional[str] = None):
     """Describes the ntfy-wrapper configuration: topics, targets and defaults."""
     conf_path = get_conf_path(conf_path)
     if not conf_path.exists():
         raise typer.BadParameter(f"Config file not found at {str(conf_path)}")
     conf = load_conf(conf_path)
     defaults = code(
-        "\n   • ".join(
+        "\n     • ".join(
             [""]
             + [
                 str(k) + " = " + str(v)
                 for k, v in conf.items()
-                if k not in ["topics", "emails"]
+                if k not in ["topics", "emails", "base_url"]
             ]
         )
     )
     print(f"🎉 Configuration file: {code(conf_path)}", style="green")
     print(f"   Topics: {code(', '.join(conf.get('topics', [])))}", style="green")
     print(f"   Emails: {code(', '.join(conf.get('emails', [])))}", style="green")
+    print(f"   Base URLs: {code(', '.join(conf.get('base_url', [])))}", style="green")
     print(f"   Defaults:{defaults}", style="green")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `ntfy_wrapper-0.1.6/ntfy_wrapper/notifier.py` & `ntfy_wrapper-0.1.7/ntfy_wrapper/notifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,26 +11,28 @@
     get_conf_path,
     load_conf,
     write_conf,
     code,
     print,
     KEYS,
 )
+import json
 
 
 class Notifier:
     """
     The main class in ntfy-wrapper.
     A Notifier(...) will handle both the configuration file and the notifications.
     """
 
     def __init__(
         self,
         topics: Optional[Union[str, List[str]]] = None,
         emails: Optional[Union[str, List[str]]] = None,
+        base_url: Optional[Union[str, List[str]]] = None,
         notify_defaults: Optional[Dict] = {},
         conf_path: Optional[Union[str, Path]] = None,
         write: Optional[bool] = True,
         warnings: Optional[bool] = True,
         verbose: Optional[bool] = True,
     ):
         """
@@ -52,36 +54,41 @@
             topics (Optional[Union[str, List[str]]], optional): String, or list of
                 strings describing the default target topics to publish to using
                 https://ntfy.sh. Remember that a topic is much like a password:
                 anyone with that string can subscribe to your notifications so
                 it's probably best you do not track any piece of code containing
                 your topics. That includes the configuration file this class creates
                 automatically (except if ``write`` is False).
-                Defaults to None, meaning a random (uuid) topic will be generated
+                Defaults to ``None``, meaning a random (uuid) topic will be generated
                 for you, and re-used next time, provided you have enabled ``write``.
             emails (Optional[Union[str, List[str]]], optional): String, or list of
                 strings describing the emails to send notifications to by default.
                 Be aware of the rate limits: https://ntfy.sh/docs/publish/#limitations
-                Defaults to None.
+                Defaults to ``None``.
+            base_url (Optional[str], optional): String or list of strings describing
+                the base url to use and send notifications to. It defaults to ``None``,
+                *i.e.* ``https://ntfy.sh`` but you can set it to a self-hosted ``ntfy``
+                instance for example. ``base_url`` can be a list of comma-separated
+                urls, in which case they will all be notified.
             notify_defaults (Optional[Dict], optional): Dict whose keys and values will
                 be default keyword arguments for the ``Notifier.notify()`` method so
                 that you don't have to write the same stuff again and again throughout
-                your code. Defaults to {}.
-            conf_path (Optional[Union[str, Path]], optional): String or pathlib.Path
+                your code. Defaults to ``{}``.
+            conf_path (Optional[Union[str, Path]], optional): String or ``pathlib.Path``
                 pointing to where the Notifier should get or create its INI
-                configuration file. Defaults to None, meaning ``$CWD/.ntfy.conf``.
+                configuration file. Defaults to ``None``, meaning ``$CWD/.ntfy.conf``.
             write (Optional[bool], optional): Whether to write the Notifier's config
                 if a new topic has to be created because none pre-exist.
-                Defaults to True.
+                Defaults to ``True``.
             warnings (Optional[bool], optional): Whether or not to print warnings,
                 in particular the version control warning if ``write`` is True (by
-                default). Defaults to True.
+                default). Defaults to ``True``.
             verbose (Optional[bool], optional): Whether to describe the Notifier after
                 its initialization from your args and the (potentially non-existing)
-                conf. Defaults to True.
+                conf. Defaults to ``True``.
         """
 
         if isinstance(topics, str):
             topics = [topics]
 
         assert isinstance(notify_defaults, dict), "notify_defaults must be a dict"
         assert all(
@@ -96,14 +103,16 @@
         # that can be overwritten by the user in the conf or the init args
         conf = load_conf(self.conf_path)
         conf.update(notify_defaults)
         if topics is not None:
             conf["topics"] = topics
         if emails is not None:
             conf["emails"] = emails
+        if base_url is not None:
+            conf["base_url"] = base_url
 
         self.conf = conf
 
         if not self.conf.get("topics"):
             if not self.conf.get("emails"):
                 self._warn(
                     "No topic set, and no email set."
@@ -147,15 +156,22 @@
                 + ", ".join([code(t) for t in self.conf["topics"]])
             )
         if self.conf.get("emails"):
             print(
                 "📧 Notifier will send emails to: "
                 + ", ".join([code(e) for e in self.conf["emails"]])
             )
-        keys = [k for k in self.conf.keys() if k not in ["topics", "emails"]]
+        if self.conf.get("base_url"):
+            print(
+                "🏡 Notifier will push to base url: "
+                + ", ".join([code(e) for e in self.conf["base_url"]])
+            )
+        keys = [
+            k for k in self.conf.keys() if k not in ["topics", "emails", "base_url"]
+        ]
         if keys:
             ml = max([len(k) for k in keys])
             print(f"🛠  {code('Notifier.notify(..)')} defaults:")
             for k in keys:
                 print(f"  • {code(k):{ml+13}} -> {code(self.conf[k])}")
         print("🗃  Its configuration is in: " + code(self.conf_path))
         return ""
@@ -169,15 +185,15 @@
         Remove topics from the Notifier's targets.
         If ``write`` is True, the configuration file is updated.
         If a topic does not exist, it is ignored.
 
         Args:
             topics (List[str]): The topics to remove.
             write (Optional[bool], optional): Whether to update the config file or not.
-                Defaults to True.
+                Defaults to ``True``.
         """
         for t in topics:
             if t not in self.conf.get("topics", []):
                 self._warn(f"Topic {t} is not in the list of topics")
             else:
                 self.conf["topics"].remove(t)
         if write:
@@ -192,50 +208,86 @@
         Remove emails from the Notifier's targets.
         If ``write`` is True, the configuration file is updated.
         If an email does not exist, it is ignored.
 
         Args:
             emails (List[str]): The emails to remove.
             write (Optional[bool], optional): Whether to update the config file or not.
-                Defaults to True.
+                Defaults to ``True``.
         """
         for e in emails:
             if e not in self.conf.get("emails", []):
                 self._warn(f"Email {e} is not in the list of emails")
             else:
                 self.conf["emails"].remove(e)
         if write:
             self.write_to_conf()
 
+    def remove_base_urls(
+        self,
+        base_urls: List[str],
+        write: Optional[bool] = True,
+    ):
+        """
+        Remove urls from the Notifier's targets.
+        If ``write`` is True, the configuration file is updated.
+        If an url does not exist, it is ignored.
+
+        Args:
+            base_urls (List[str]): The base_urls to remove.
+            write (Optional[bool], optional): Whether to update the config file or not.
+                Defaults to ``True``.
+        """
+        for e in base_urls:
+            if e not in self.conf.get("base_url", []):
+                self._warn(f"URL {e} is not in the list of base_url")
+            else:
+                self.conf["base_url"].remove(e)
+        if write:
+            self.write_to_conf()
+
     def remove_all_topics(self, write: Optional[bool] = True):
         """
         Remove all emails from the Notifier's targets.
         If ``write`` is True, the configuration file is updated.
 
         Args:
             write (Optional[bool], optional): Whether to update the config file or not.
-                Defaults to True.
+                Defaults to ``True``.
         """
         self.conf["topics"] = []
         if write:
             self.write_to_conf()
 
     def remove_all_emails(self, write: Optional[bool] = True):
         """
         Remove all emails from the Notifier's targets.
         If ``write`` is True, the configuration file is updated.
 
         Args:
             write (Optional[bool], optional): Whether to update the config file or not.
-                Defaults to True.
+                Defaults to ``True``.
         """
         self.conf["emails"] = []
         if write:
             self.write_to_conf()
 
+    def remove_all_base_urls(self, write: Optional[bool] = True):
+        """
+        Remove all base urls from the Notifier's targets.
+        If ``write`` is True, the configuration file is updated.
+
+        Args:
+            write (Optional[bool], optional): Whether to update the config file or not.
+                Defaults to ``True``.
+        """
+        self.conf["base_url"] = []
+        if write:
+            self.write_to_conf()
+
     def write_to_conf(self):
         """
         Write the topics to the configuration file.
         """
         self._warn(
             "❗️ Warning: your configuration may contain sensitive data. "
             + "Make sure it is ignored by your version control system "
@@ -281,15 +333,16 @@
         if write:
             self.write_to_conf()
 
     def notify(
         self,
         message: str,
         topics: Optional[Union[str, List[str]]] = None,
-        emails: Optional[List[str]] = None,
+        emails: Optional[Union[str, List[str]]] = None,
+        base_url: Optional[Union[str, List[str]]] = None,
         title: Optional[str] = None,
         priority: Optional[int] = None,
         tags: Optional[Union[str, List[str]]] = None,
         click: Optional[str] = None,
         attach: Optional[str] = None,
         actions: Optional[Union[str, List[str]]] = None,
         icon: Optional[str] = None,
@@ -301,66 +354,95 @@
         .. note::
             Refer to the ntfy documentation more details about all those options:
             https://ntfy.sh/docs/publish/
 
         The ``defaults`` you may have used in the ``init()`` method are used here.
         You can override them by passing the corresponding arguments.
 
+        In other words: ``arg`` > ``self.conf`` > ``defaults``.
+
         If ``topics`` is None, the topics are taken from the configuration file.
         If ``emails`` is not None, the notification is sent by email to the given
         addresses.
         If ``emails`` have been specified in the configuration file, they are used by
         default.
         Set ``emails=""`` to disable emails even if there are some in the configuration.
 
         .. warning::
             You cannot send both a string message and a file attachment.
 
         Args:
             message (str): The message to send.
             topics (Optional[Union[str, List[str]]], optional): Target topics to notify.
-                Defaults to None.
+                Defaults to ``None``.
+            emails (Optional[Union[str, List[str]]], optional): Target emails to send
+                notifications to. Defaults to ``None``.
+            base_url (Optional[Union[str, List[str]]], optional): The base URL to use
+                for the API. Can be a coma-separated list of URLs. Defaults to ``None``,
+                i.e. ``https://ntfy.sh`` if ``base_url`` is neither an arg nor in the
+                config.
             title (Optional[str], optional): The notifications' title.
                 Defaults to "From ntfy_wrapper".
             priority (Optional[int], optional): The notifications' priority.
-                Defaults to None.
+                Defaults to ``None``.
             tags (Optional[Union[str, List[str]]], optional): The notifications' tags.
-                Defaults to None.
+                Defaults to ``None``.
             click (Optional[str], optional):  URL to open when a notification is
-                clicked. Defaults to None.
+                clicked. Defaults to ``None``.
             attach (Optional[str], optional): Attachment to send: either a local image
-                file or an URL pointing to one. Defaults to None.
+                file or an URL pointing to one. Defaults to ``None``.
             actions (Optional[Union[str, List[str]]], optional): A string or list of
                 strings describing actions as per:
                 https://ntfy.sh/docs/publish/#using-a-header
-                Defaults to None.
-            emails (Optional[List[str]], optional): _description_. Defaults to None.
+                Defaults to ``None``.
             icon (Optional[str], optional): The notifications' icon as a URL to a
-                remote file. Defaults to None.
+                remote file. Defaults to ``None``.
+            debug (Optional[bool], optional): Whether to print debug information or not.
+                Defaults to ``False``.
 
         Raises:
             ValueError: The user cannot specify both ``attach`` and ``message``
 
         Returns:
             List[str]: A list of the targets notifications have been dispatched to:
                 one for each topic and one for each email.
         """
         defaults = {
             k.capitalize(): v
             for k, v in self.conf.items()
-            if k not in {"topics", "emails"}
+            if k not in {"topics", "emails", "base_url"}
         }
         headers = {**defaults, "priority": priority}
         headers = {k: v for k, v in headers.items() if v is not None}
 
         if attach and message:
             raise ValueError("You cannot specify both `attach` and `message`")
 
         use_PUT = False
 
+        if base_url is None:
+            base_url = self.conf.get("base_url", ["https://ntfy.sh"])
+        if isinstance(base_url, str):
+            if "," in base_url:
+                base_urls = [u.strip() for u in base_url.split(",")]
+            else:
+                base_urls = [base_url]
+        if not isinstance(base_urls, list) or not base_urls or not base_urls[0]:
+            self._warn(
+                "\nNo base URL specified in conf or as argument,"
+                + " using https://ntfy.sh\n"
+            )
+            base_urls = ["https://ntfy.sh"]
+
+        for u in base_urls:
+            if not u.startswith("http"):
+                self._warn(f"\nBe careful, base url does not start with `http` : {u}\n")
+
+        base_urls = [u[:-1] if u.endswith("/") else u for u in base_urls]
+
         if title is not None:
             headers["Title"] = title
 
         if click is not None:
             headers["Click"] = click
         if icon is not None:
             headers["Icon"] = icon
@@ -391,52 +473,56 @@
             if isinstance(topics, str):
                 topics = [topics]
         else:
             topics = self.conf.get("topics", [])
 
         assert isinstance(emails, list)
         assert isinstance(topics, list)
+        assert isinstance(base_urls, list)
 
         dispatchs = []
-
-        for dtype, dest in [("topic", t) for t in topics] + [
-            ("email", e) for e in emails
-        ]:
-            h = headers.copy()
-
-            if dtype == "email":
-                h["Email"] = dest
-                url = "https://ntfy.sh/alerts"
-            else:
-                url = f"https://ntfy.sh/{dest}"
-
-            dispatchs.append(dest)
-
-            if not use_PUT:
-                if debug:
-                    print(f"Sending {message} to {dest}:")
-                    print("    target url: ", url)
-                    print("    message: ", message.encode("utf-8"))
-                    print("    headers: ", h)
-                requests.post(
-                    url,
-                    data=message.encode("utf-8"),
-                    headers=h,
-                )
-            else:
-                h["Filename"] = Path(attach).name
-                requests.put(
-                    url,
-                    data=open(attach, "rb"),
-                    headers=h,
-                )
+        for base_url in base_urls:
+            for dtype, dest in [("topic", t) for t in topics] + [
+                ("email", e) for e in emails
+            ]:
+                h = headers.copy()
+
+                if dtype == "email":
+                    h["Email"] = dest
+                    url = f"{base_url}/alerts"
+                else:
+                    url = f"{base_url}/{dest}"
+
+                dispatchs.append(dest)
+
+                if not use_PUT:
+                    if debug:
+                        print(f"➡️ Sending `{message}` to `{dest}`:")
+                        print("    target url: ", url)
+                        print("    message: ", message.encode("utf-8"))
+                        print(
+                            "    headers: ",
+                            "\n    ".join(json.dumps(h, indent=2).splitlines()),
+                        )
+                    requests.post(
+                        url,
+                        data=message.encode("utf-8"),
+                        headers=h,
+                    )
+                else:
+                    h["Filename"] = Path(attach).name
+                    requests.put(
+                        url,
+                        data=open(attach, "rb"),
+                        headers=h,
+                    )
 
         if debug:
             print(
-                "Debug mode: make sure the above messages,"
+                "\nDebug mode: make sure the above messages,"
                 + " headers and targets are correct."
             )
             print(
                 "In particular, no `None` should appear in the headers, and all their"
                 + " keys should start with an uppercase letter."
             )
             print(
```

### Comparing `ntfy_wrapper-0.1.6/ntfy_wrapper/utils.py` & `ntfy_wrapper-0.1.7/ntfy_wrapper/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ⇩
 Example:
 -----------------------------------------------------------------------------------------
 # For Notifier(emails=..., topics=...)
 [notifier_init]
 topics = my-secret-topic-1, mysecrettopic2
 emails = you@foo.bar
+base_url = https://ntfy.your-server.io
 
 # For Notifier.notify(title=..., priority=..., etc.)
 [notify_defaults]
 title = Message from ntfy-wrapper
 priority = 0
 tags = fire
 click =
@@ -65,15 +66,15 @@
     Finds a path to the configuration file.
     If a directory is provided, the config file will be named ".ntfy.conf"
     If the path is not provided, it will look for the file in the
     current working directory,
 
     Args:
         conf_path (Optional[Union[str, Path]], optional): Where to look for the config
-            file. Defaults to None.
+            file. Defaults to ``None``.
 
     Returns:
         Path: _description_
     """
     if conf_path is None:
         path = Path.cwd()
     elif isinstance(conf_path, str):
@@ -90,15 +91,15 @@
 def load_conf(conf_path: Optional[Union[str, Path]] = None) -> dict:
     """
     Loads a config file from the given path.
     Expects the INI format and will use configparser.
 
     Args:
         conf_path (Optional[Union[str, Path]], optional): Where to load the conf
-        from. Defaults to None.
+        from. Defaults to ``None``.
 
     Returns:
         dict: The configuration as a dictionary.
     """
     path = get_conf_path(conf_path)
     if path.exists():
         config = configparser.ConfigParser()
@@ -109,14 +110,19 @@
                 conf["topics"] = [
                     t.strip() for t in config.get("notifier_init", "topics").split(",")
                 ]
             if "emails" in config["notifier_init"]:
                 conf["emails"] = [
                     e.strip() for e in config.get("notifier_init", "emails").split(",")
                 ]
+            if "base_url" in config["notifier_init"]:
+                conf["base_url"] = [
+                    e.strip()
+                    for e in config.get("notifier_init", "base_url").split(",")
+                ]
         if config.has_section("notify_defaults"):
             conf.update(dict(config["notify_defaults"]))
         return conf
 
     return {
         "title": "Message from ntfy-wrapper",
         "tags": "fire",
@@ -135,26 +141,29 @@
     Args:
         conf_path (Path): The path to the configuration file.
         conf (Dict[str, Union[str, List[str]]]): The configuration to write.
     """
     conf = deepcopy(conf)
     topics = conf.pop("topics", None)
     emails = conf.pop("emails", None)
+    base_url = conf.pop("base_url", None)
 
     config = configparser.ConfigParser(allow_no_value=True)
 
     config.add_section("about")
     for line in DOCSTRING.split("\n")[1:]:
         config.set("about", ("# " + line).strip())
 
     config.add_section("notifier_init")
     if topics:
         config.set("notifier_init", "topics", ",".join(topics))
     if emails:
         config.set("notifier_init", "emails", ",".join(emails))
+    if base_url:
+        config.set("notifier_init", "base_url", ",".join(base_url))
 
     config.add_section("notify_defaults")
     for k, v in conf.items():
         config.set("notify_defaults", k, v)
 
     config.write(conf_path.open("w"))
```

### Comparing `ntfy_wrapper-0.1.6/pyproject.toml` & `ntfy_wrapper-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "ntfy-wrapper"
-version = "0.1.6"
+version = "0.1.7"
 description = "Fast & Free notifications for your code: Python wrapper around the ntfy.sh notifications service."
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
-readme = "README.md"
+readme = 'README.md'
 packages = [{include = "ntfy_wrapper"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 xkcdpass = "^1.19.3"
```

### Comparing `ntfy_wrapper-0.1.6/setup.py` & `ntfy_wrapper-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'xkcdpass>=1.19.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['py-ntfy = ntfy_wrapper.cli:app']}
 
 setup_kwargs = {
     'name': 'ntfy-wrapper',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Fast & Free notifications for your code: Python wrapper around the ntfy.sh notifications service.',
-    'long_description': '\n<p align="center">\n    <a href="https://github.com/vict0rsch/ntfy-wrapper" target="_blank">\n        <img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/ntfy-txt.png">\n    </a>\n</p>\n<p align="center">\n    <a href="https://pypi.org/project/ntfy-wrapper/"><img src="https://img.shields.io/badge/pypi%20package-0.1.6-yellowgreen" alt="PyPI version" height="18"></a>\n    <a href="https://ntfy-wrapper.readthedocs.io/en/latest/index.html"><img src="https://img.shields.io/badge/docs-read%20the%20docs-blue" alt="PyPI version" height="18"></a>\n    <a href="https://github.com/vict0rsch/ntfy-wrapper/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"><img src="https://img.shields.io/github/issues-raw/vict0rsch/ntfy-wrapper" alt="Open Issues" height="18"></a>\n    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/codestyle-black-red" alt="Black code style" height="18"></a>\n    <a href="https://github.com/vict0rsch/ntfy-wrapper/blob/main/LICENSE><img src="https://img.shields.io/github/license/vict0rsch/ntfy-wrapper" alt="License" height="18"></a>\n</p>\n\n`ntfy-wrapper` is a free and hassle-free customizable notifier for Python. No login, no API token, no fees, no bullshit.\n\nIt\'s actually a simple Python wrapper around [`ntfy`](https://ntfy.sh). Kudos to them ❤️\n\nYou can now **send** notification from your Python code and **receive** them on your computer through a [Web App](https://ntfy.sh/app) or a [CLI](https://ntfy.sh/docs/subscribe/cli/), or [on your phone with a dedicated app](https://ntfy.sh/docs/subscribe/phone/)!\n\nAgain, all credit to [`ntfy`](https://ntfy.sh).\n\n## Install\n\nInstall `ntfy-wrapper` with `pip`:\n\n```bash\npip install ntfy-wrapper\n```\n\nDependencies:\n\n* `requests` for easy HTTP requests and interacting with the `ntfy.sh` API\n* `typer` for a powerful and beautiful CLI\n* `xkcdpass` to generate secure but human-friendly topics[^1]\n\n## Why?\n\nImagine you execute jobs on a shared cluster. They are in a queue. You get notified when they start. You get notified if there\'s an error. You get notified with the final performance of your model and if you click on the notification, you have access to the online logs from wandb or comet.ml.\n\nThat\'s just one scenario inspired from my work in AI, but really you can use it in any context!\n\n## Getting Started\n\n```python\nfrom ntfy_wrapper import Notifier\n\nif __name__ == "__main__":\n\n    ntfy = Notifier(notify_defaults={"title": "Your Project Name"})\n    # IFF this is the first call to `ntfy_wrapper` in your project, this line ^\n    # will print a topic id.\n    # It will also write the topic id to `.ntfy.conf` so this only happens once!\n    #\n    # Use one of those methods (from the print or the conf file) to copy the topic id\n    # and use it to subscribe to notifications from the web or mobile apps.\n    #\n    # You can also use the command-line `$ py-ntfy init` before executing your code\n    # and the same process will happen (new topic + conf file)\n    #\n    # Note: anyone with your topic id can subscribe to your notification. It\'s probably\n    # best to *exclude* the configuration file from version control.\n\n    ntfy("Job has been allocated, starting Model training")\n\n    try:\n        results = do_some_stuff()\n        if results["metric"] > threshold:\n            ntfy(\n                f"Great model! Its metric is {results[\'metric\']:.3f}",\n                tags="white_check_mark",  # this is the ✅ emoji\n                click=results["online_run_url"],\n            )\n        else:\n            ntfy(f"Done, but not great ({results[\'metric\']:.3f})", tags="disappointed")\n    except Exception as e:\n        ntfy.notify(f"Error! -> {str(e)}", priority=4, emails="you@foo.bar")\n```\n\nNote `ntfy(message)` is equivalent to `ntfy.notify(message)`, the former is an alias of the latter.\n\n**If you do not receive notifications** after you\'ve made sure you\'ve subscribed to the exact topic used by your `Notifier`, it\'s probably because the request being sent out is malformed. Investigate using `debug=True` in the `notify()` call (*e.g.* : `ntfy(message, debug=True)`).\n\n## User Guide\n\nThe central concept is **"topics"**. It\'s basically an ID used to publish/subscribe to notifications. You should keep it secret and not easily guessable because ***anyone with the topic id can subscribe to your notifications***. In particular, you should add `.ntfy.conf` to `.gitignore`.\n\nIn short, `ntfy-wrapper` will *publish* to a *topic* and you\'ll have to *subscribe* to that same topic in order to receive the notification. You can receive your notification:\n\n* On your computer\n  * By opening a [local web app](https://ntfy.sh/app) <a href="https://ntfy.sh/app"><img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/webapp.png" height="400"></a>\n  * By setting up the [`ntfy` CLI tool](https://ntfy.sh/docs/subscribe/cli/)\n* On your phone\n  * By installing [a mobile app](https://ntfy.sh/docs/subscribe/phone/)\n\n### How to use\n\n1. Create topics in one of the following ways:\n   1. configure one manually\n   2. In a Python console use `ntfy_wrapper.utils.generate_topic()` to get a secure unique and human-readable topic (eg: `winter-abide-dinghy-wand`)\n   3. From the command-line use `$ py-ntfy new-topic` to get a similar topic. Add `--save` to add it to the configuration.\n2. Tell the `Notifier` to use this topic in one of the following ways:\n   1. In your code `Notifier(topics=your_topic)` or `Notifier(topics=[topic1, topic2])`\n   2. Using a **configuration file**\n      1. A configuration file will be created by default when constructing a `Notifier` *except* if you add `write=False` to the `Notifier.__init__` arguments\n      2. The configuration file is used to hold default values for:\n         1. `targets`, i.e. a list of comma-separated `topics` and a list of comma-separated `emails`\n         2. `message_defaults` which are default values used when calling `.notify(...)`\n      3. You can also use `$ py-ntfy init` to initialize your `ntfy-wrapper` configuration\n   3. From the command-line with `$ py-ntfy add topic your-topic`\n3. Setup defaults in one of the following ways\n   1. By editing the config file\n   2. By using the [`py-ntfy` command-line tool](#command-line)\n4. Explore notification options by referring to the original [`ntfy` docs](https://ntfy.sh/docs/publish/)\n\n<a href="https://ntfy.sh/app"><img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/mermaid.png"></a>\n\n## Configuration file\n\n`ntfy-wrapper` uses the INI standard along with `configparser` to parse the configuration file. It expects 2 sections:\n\n1. `[notifier_init]` with optional fields `emails = ` and `topics = ` to define systematic targets for the notification instead of putting them in your Python code\n2. `[notify_defaults]` with optional fields listed below, which will define default parameters used by `Notifier.notify(...)`. For instance you can set default `title` and `tags` for your code\'s `.notify(...)` calls and override them at specific locations with keyword arguments `.notify(title="Non-default title")`\n   1. The behavior of the `title`, `priority`, `tags`, `click`, `attach`, `actions` and `icon` keys is described in the [`ntfy` docs](https://ntfy.sh/docs/publish/)\n\n```ini\n# For Notifier(emails=..., topics=...)\n[notifier_init]\ntopics = my-secret-topic-1, mysecrettopic2\nemails = you@foo.bar\n\n# For Notifier.notify(title=..., priority=..., etc.)\n[notify_defaults]\ntitle = Message from ntfy-wrapper\npriority = 0\ntags = fire\nclick =\nattach =\nactions =\nicon = https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/logo.png\n```\n\n## Command-line\n\n`ntfy_wrapper` comes with a command-line interface called `py-ntfy`. It uses the great Python CLI tool [`Typer`](https://typer.tiangolo.com/). Its goal is to interact with `ntfy-wrapper`\'s configuration in a user-friendly way. It is different in that sense to the original [`ntfy` CLI tool](https://ntfy.sh/docs/subscribe/cli/) which is more generic.\n\n* Get help\n\n    ```bash\n    $ py-ntfy --help\n    Usage: py-ntfy [OPTIONS] COMMAND [ARGS]...\n\n    ╭─ Options ────────────────────────────────────────────────────────────────────────────────╮\n    │ --install-completion          Install completion for the current shell.                  │\n    │ --show-completion             Show completion for the current shell, to copy it or       │\n    │                               customize the installation.                                │\n    │ --help                        Show this message and exit.                                │\n    ╰──────────────────────────────────────────────────────────────────────────────────────────╯\n    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────╮\n    │ add        [command sub-group] Add a new notification target or a default notification   │\n    │            value. Run `$ py-ntfy add --help` for more info.                              │\n    │ clean      Removes the configuration file. Use --conf-path to specify a path to the      │\n    │            configuration file. Use --force to skip the confirmation prompt.              │\n    │ init       Initializes the configuration file. It should NOT be tracked by version       │\n    │            control in order to protect the topic ID. Use --conf-path to specify a path   │\n    │            to the configuration file. Use --force to overwrite an existing configuration │\n    │            file.                                                                         │\n    │ new-topic  Generates a random topic name and saves it to the config file if you use the  │\n    │            --save option.                                                                │\n    │ remove     [command sub-group] Remove a notification target or a default notification    │\n    │            value. Run `$ py-ntfy remove --help` for more info.                           │\n    │ send       Sends a notification to the given emails and topics. Optional command-line    │\n    │            arguments can be passed to override the defaults in the config file and       │\n    │            customize the message options. Refer to https://ntfy.sh/docs/publish to       │\n    │            understand the options. Run `py-ntfy send --help` to see the available        │\n    │            options.                                                                      │\n    ╰──────────────────────────────────────────────────────────────────────────────────────────╯\n\n    $ py-ntfy add --help\n    (similar output)\n\n    $ py-ntfy add default --help\n    (similar output)\n\n    $ py-ntfy remove --help\n    (similar output)\n    ```\n\n* Initialize the configuration file\n\n    ```bash\n    $ py-ntfy init\n    🔑 Your first topic is `aloe-corset-stream-alto`. Use it to subscribe to notifications!\n    🎉 Config file created at /path/to/repo/.ntfy.conf\n    ```\n\n* Add a topic or an email\n\n    ```bash\n    $ py-ntfy add topic some-secret-string-for-your-topic\n    🎉 Topic `some-secret-string-for-your-topic` added to /path/to/repo/.ntfy.conf\n\n    $ py-ntfy add email you@foo.bar\n    🎉 Email you@foo.bar added to /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n    ```\n\n* Add a default value for the `.notify(...)` calls\n\n    ```bash\n    $ py-ntfy add default key value\n    🎉 Default key=value added to /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n    ```\n\n* Remove items by simply replacing `add` by `remove`\n\n    ```bash\n    $ py-ntfy remove default key\n    🎉 Default key=value removed from /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n\n    $ py-ntfy remove email hello@you.com\n    Email hello@you.com does not exist. Ignoring.\n    ```\n\n* Generate a new topic with `new-topic` and add it to your configuration with `--save`\n\n    ```bash\n    $ py-ntfy new-topic --save\n    🎉 Topic nutty-tiling-clear-parlor added to /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n    ```\n\n* Send a notification from the command-line with `send`\n\n    ```bash\n    $ py-ntfy send "hello" --topics frays-errant-acting-huddle --title "This is Victor" --click "https://9gag.com"\n    🎉 Notification sent to frays-errant-acting-huddle, you@foo.bar\n    ```\n\n* Change the default configuration path for any command with the option `--conf-path`\n  * Specify a directory  `--conf-path path/to/conf/directory` and `.ntfy.conf` will be created there\n  * Specify a file `--conf-path path/to/file.conf` and that will be used as a configuration file\n\n## Todo\n\n* [x] Better readme and doc\n* [x] CLI\n* [ ] Screenshots\n* [ ] `requests` timeout or non-blocking\n\n<br/>\n\n---\n\n<br/>\n\n[^1]: cf [xkcd936](https://xkcd.com/936/)\n\n<p align="center"><img src="https://imgs.xkcd.com/comics/password_strength.png"></p>\n',
+    'long_description': '\n<p align="center">\n    <a href="https://github.com/vict0rsch/ntfy-wrapper" target="_blank">\n        <img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/ntfy-txt.png">\n    </a>\n</p>\n<p align="center">\n    <a href="https://pypi.org/project/ntfy-wrapper/"><img src="https://img.shields.io/badge/pypi%20package-0.1.7-yellowgreen" alt="PyPI version" height="18"></a>\n    <a href="https://ntfy-wrapper.readthedocs.io/en/latest/index.html"><img src="https://img.shields.io/badge/docs-read%20the%20docs-blue" alt="PyPI version" height="18"></a>\n    <a href="https://github.com/vict0rsch/ntfy-wrapper/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"><img src="https://img.shields.io/github/issues-raw/vict0rsch/ntfy-wrapper" alt="Open Issues" height="18"></a>\n    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/codestyle-black-red" alt="Black code style" height="18"></a>\n    <a href="https://github.com/vict0rsch/ntfy-wrapper/blob/main/LICENSE><img src="https://img.shields.io/github/license/vict0rsch/ntfy-wrapper" alt="License" height="18"></a>\n</p>\n\n`ntfy-wrapper` is a free and hassle-free customizable notifier for Python. No login, no API token, no fees, no bullshit.\n\nIt\'s actually a simple Python wrapper around [`ntfy`](https://ntfy.sh). Kudos to them ❤️\n\nYou can now **send** notification from your Python code and **receive** them on your computer through a [Web App](https://ntfy.sh/app) or a [CLI](https://ntfy.sh/docs/subscribe/cli/), or [on your phone with a dedicated app](https://ntfy.sh/docs/subscribe/phone/)!\n\nAgain, all credit to [`ntfy`](https://ntfy.sh).\n\n## Install\n\nInstall `ntfy-wrapper` with `pip`:\n\n```bash\npip install ntfy-wrapper\n```\n\nDependencies:\n\n* `requests` for easy HTTP requests and interacting with the `ntfy.sh` API\n* `typer` for a powerful and beautiful CLI\n* `xkcdpass` to generate secure but human-friendly topics[^1]\n\n## Why?\n\nImagine you execute jobs on a shared cluster. They are in a queue. You get notified when they start. You get notified if there\'s an error. You get notified with the final performance of your model and if you click on the notification, you have access to the online logs from wandb or comet.ml.\n\nThat\'s just one scenario inspired from my work in AI, but really you can use it in any context!\n\n## Getting Started\n\n```python\nfrom ntfy_wrapper import Notifier\n\nif __name__ == "__main__":\n\n    ntfy = Notifier(notify_defaults={"title": "Your Project Name"})\n    # IFF this is the first call to `ntfy_wrapper` in your project, this line ^\n    # will print a topic id.\n    # It will also write the topic id to `.ntfy.conf` so this only happens once!\n    #\n    # Use one of those methods (from the print or the conf file) to copy the topic id\n    # and use it to subscribe to notifications from the web or mobile apps.\n    #\n    # You can also use the command-line `$ py-ntfy init` before executing your code\n    # and the same process will happen (new topic + conf file)\n    #\n    # Note: anyone with your topic id can subscribe to your notification. It\'s probably\n    # best to *exclude* the configuration file from version control.\n\n    ntfy("Job has been allocated, starting Model training")\n\n    try:\n        results = do_some_stuff()\n        if results["metric"] > threshold:\n            ntfy(\n                f"Great model! Its metric is {results[\'metric\']:.3f}",\n                tags="white_check_mark",  # this is the ✅ emoji\n                click=results["online_run_url"],\n            )\n        else:\n            ntfy(f"Done, but not great ({results[\'metric\']:.3f})", tags="disappointed")\n    except Exception as e:\n        ntfy.notify(f"Error! -> {str(e)}", priority=4, emails="you@foo.bar")\n```\n\nNote `ntfy(message)` is equivalent to `ntfy.notify(message)`, the former is an alias of the latter.\n\n**If you do not receive notifications** after you\'ve made sure you\'ve subscribed to the exact topic used by your `Notifier`, it\'s probably because the request being sent out is malformed. Investigate using `debug=True` in the `notify()` call (*e.g.* : `ntfy(message, debug=True)`).\n\n## User Guide\n\nThe central concept is **"topics"**. It\'s basically an ID used to publish/subscribe to notifications. You should keep it secret and not easily guessable because ***anyone with the topic id can subscribe to your notifications***. In particular, you should add `.ntfy.conf` to `.gitignore`.\n\nIn short, `ntfy-wrapper` will *publish* to a *topic* and you\'ll have to *subscribe* to that same topic in order to receive the notification. You can receive your notification:\n\n* On your computer\n  * By opening a [local web app](https://ntfy.sh/app) <a href="https://ntfy.sh/app"><img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/webapp.png" height="400"></a>\n  * By setting up the [`ntfy` CLI tool](https://ntfy.sh/docs/subscribe/cli/)\n* On your phone\n  * By installing [a mobile app](https://ntfy.sh/docs/subscribe/phone/)\n\n### How to use\n\n1. Create topics in one of the following ways:\n   1. configure one manually\n   2. In a Python console use `ntfy_wrapper.utils.generate_topic()` to get a secure unique and human-readable topic (eg: `winter-abide-dinghy-wand`)\n   3. From the command-line use `$ py-ntfy new-topic` to get a similar topic. Add `--save` to add it to the configuration.\n2. Tell the `Notifier` to use this topic in one of the following ways:\n   1. In your code `Notifier(topics=your_topic)` or `Notifier(topics=[topic1, topic2])`\n   2. Using a **configuration file**\n      1. A configuration file will be created by default when constructing a `Notifier` *except* if you add `write=False` to the `Notifier.__init__` arguments\n      2. The configuration file is used to hold default values for:\n         1. `targets`, i.e. a list of comma-separated `topics` and a list of comma-separated `emails`\n         2. `message_defaults` which are default values used when calling `.notify(...)`\n      3. You can also use `$ py-ntfy init` to initialize your `ntfy-wrapper` configuration\n   3. From the command-line with `$ py-ntfy add topic your-topic`\n3. Setup defaults in one of the following ways\n   1. By editing the config file\n   2. By using the [`py-ntfy` command-line tool](#command-line)\n4. Explore notification options by referring to the original [`ntfy` docs](https://ntfy.sh/docs/publish/)\n\n<a href="https://ntfy.sh/app"><img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/mermaid.png"></a>\n\n## Configuration file\n\n`ntfy-wrapper` uses the INI standard along with `configparser` to parse the configuration file. It expects 2 sections:\n\n1. `[notifier_init]` with optional fields `emails = `, `topics = ` and `base_url = ` to define systematic targets for the notification instead of putting them in your Python code. `base_url` allows to push to a different `ntfy` server than the default `https://ntfy.sh`.\n2. `[notify_defaults]` with optional fields listed below, which will define default parameters used by `Notifier.notify(...)`. For instance you can set default `title` and `tags` for your code\'s `.notify(...)` calls and override them at specific locations with keyword arguments `.notify(title="Non-default title")`\n   1. The behavior of the `title`, `priority`, `tags`, `click`, `attach`, `actions` and `icon` keys is described in the [`ntfy` docs](https://ntfy.sh/docs/publish/)\n\n```ini\n# For Notifier(emails=..., topics=...)\n[notifier_init]\ntopics = my-secret-topic-1, mysecrettopic2\nemails = you@foo.bar\nbase_url = https://custom-ntfy-instance.io\n\n# For Notifier.notify(title=..., priority=..., etc.)\n[notify_defaults]\ntitle = Message from ntfy-wrapper\npriority = 0\ntags = fire\nclick =\nattach =\nactions =\nicon = https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/logo.png\n```\n\n## Command-line\n\n`ntfy_wrapper` comes with a command-line interface called `py-ntfy`. It uses the great Python CLI tool [`Typer`](https://typer.tiangolo.com/). Its goal is to interact with `ntfy-wrapper`\'s configuration in a user-friendly way. It is different in that sense to the original [`ntfy` CLI tool](https://ntfy.sh/docs/subscribe/cli/) which is more generic.\n\n* Get help\n\n    ```bash\n    $ py-ntfy --help\n    Usage: py-ntfy [OPTIONS] COMMAND [ARGS]...\n\n    ╭─ Options ────────────────────────────────────────────────────────────────────────────────╮\n    │ --install-completion          Install completion for the current shell.                  │\n    │ --show-completion             Show completion for the current shell, to copy it or       │\n    │                               customize the installation.                                │\n    │ --help                        Show this message and exit.                                │\n    ╰──────────────────────────────────────────────────────────────────────────────────────────╯\n    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────╮\n    │ add        [command sub-group] Add a new notification target or a default notification   │\n    │            value. Run `$ py-ntfy add --help` for more info.                              │\n    │ clean      Removes the configuration file. Use --conf-path to specify a path to the      │\n    │            configuration file. Use --force to skip the confirmation prompt.              │\n    │ init       Initializes the configuration file. It should NOT be tracked by version       │\n    │            control in order to protect the topic ID. Use --conf-path to specify a path   │\n    │            to the configuration file. Use --force to overwrite an existing configuration │\n    │            file.                                                                         │\n    │ new-topic  Generates a random topic name and saves it to the config file if you use the  │\n    │            --save option.                                                                │\n    │ remove     [command sub-group] Remove a notification target or a default notification    │\n    │            value. Run `$ py-ntfy remove --help` for more info.                           │\n    │ send       Sends a notification to the given emails and topics. Optional command-line    │\n    │            arguments can be passed to override the defaults in the config file and       │\n    │            customize the message options. Refer to https://ntfy.sh/docs/publish to       │\n    │            understand the options. Run `py-ntfy send --help` to see the available        │\n    │            options.                                                                      │\n    ╰──────────────────────────────────────────────────────────────────────────────────────────╯\n\n    $ py-ntfy add --help\n    (similar output)\n\n    $ py-ntfy add default --help\n    (similar output)\n\n    $ py-ntfy remove --help\n    (similar output)\n    ```\n\n* Initialize the configuration file\n\n    ```bash\n    $ py-ntfy init\n    🔑 Your first topic is `aloe-corset-stream-alto`. Use it to subscribe to notifications!\n    🎉 Config file created at /path/to/repo/.ntfy.conf\n    ```\n\n* Add a topic or an email\n\n    ```bash\n    $ py-ntfy add topic some-secret-string-for-your-topic\n    🎉 Topic `some-secret-string-for-your-topic` added to /path/to/repo/.ntfy.conf\n\n    $ py-ntfy add email you@foo.bar\n    🎉 Email you@foo.bar added to /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n    ```\n\n* Add a default value for the `.notify(...)` calls\n\n    ```bash\n    $ py-ntfy add default key value\n    🎉 Default key=value added to /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n    ```\n\n* Remove items by simply replacing `add` by `remove`\n\n    ```bash\n    $ py-ntfy remove default key\n    🎉 Default key=value removed from /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n\n    $ py-ntfy remove email hello@you.com\n    Email hello@you.com does not exist. Ignoring.\n    ```\n\n* Generate a new topic with `new-topic` and add it to your configuration with `--save`\n\n    ```bash\n    $ py-ntfy new-topic --save\n    🎉 Topic nutty-tiling-clear-parlor added to /Users/.../vict0rsch/ntfy-wrapper/.ntfy.conf\n    ```\n\n* Send a notification from the command-line with `send`\n\n    ```bash\n    $ py-ntfy send "hello" --topics frays-errant-acting-huddle --title "This is Victor" --click "https://9gag.com"\n    🎉 Notification sent to frays-errant-acting-huddle, you@foo.bar\n    ```\n\n* Change the default configuration path for any command with the option `--conf-path`\n  * Specify a directory  `--conf-path path/to/conf/directory` and `.ntfy.conf` will be created there\n  * Specify a file `--conf-path path/to/file.conf` and that will be used as a configuration file\n\n## Todo\n\n* [x] Better readme and doc\n* [x] CLI\n* [ ] Screenshots\n* [ ] `requests` timeout or non-blocking\n\n<br/>\n\n---\n\n<br/>\n\n[^1]: cf [xkcd936](https://xkcd.com/936/)\n\n<p align="center"><img src="https://imgs.xkcd.com/comics/password_strength.png"></p>\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ntfy_wrapper-0.1.6/PKG-INFO` & `ntfy_wrapper-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntfy-wrapper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Fast & Free notifications for your code: Python wrapper around the ntfy.sh notifications service.
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 
 <p align="center">
     <a href="https://github.com/vict0rsch/ntfy-wrapper" target="_blank">
         <img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/ntfy-txt.png">
     </a>
 </p>
 <p align="center">
-    <a href="https://pypi.org/project/ntfy-wrapper/"><img src="https://img.shields.io/badge/pypi%20package-0.1.6-yellowgreen" alt="PyPI version" height="18"></a>
+    <a href="https://pypi.org/project/ntfy-wrapper/"><img src="https://img.shields.io/badge/pypi%20package-0.1.7-yellowgreen" alt="PyPI version" height="18"></a>
     <a href="https://ntfy-wrapper.readthedocs.io/en/latest/index.html"><img src="https://img.shields.io/badge/docs-read%20the%20docs-blue" alt="PyPI version" height="18"></a>
     <a href="https://github.com/vict0rsch/ntfy-wrapper/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"><img src="https://img.shields.io/github/issues-raw/vict0rsch/ntfy-wrapper" alt="Open Issues" height="18"></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/codestyle-black-red" alt="Black code style" height="18"></a>
     <a href="https://github.com/vict0rsch/ntfy-wrapper/blob/main/LICENSE><img src="https://img.shields.io/github/license/vict0rsch/ntfy-wrapper" alt="License" height="18"></a>
 </p>
 
 `ntfy-wrapper` is a free and hassle-free customizable notifier for Python. No login, no API token, no fees, no bullshit.
@@ -134,23 +134,24 @@
 
 <a href="https://ntfy.sh/app"><img src="https://raw.githubusercontent.com/vict0rsch/ntfy-wrapper/main/assets/mermaid.png"></a>
 
 ## Configuration file
 
 `ntfy-wrapper` uses the INI standard along with `configparser` to parse the configuration file. It expects 2 sections:
 
-1. `[notifier_init]` with optional fields `emails = ` and `topics = ` to define systematic targets for the notification instead of putting them in your Python code
+1. `[notifier_init]` with optional fields `emails = `, `topics = ` and `base_url = ` to define systematic targets for the notification instead of putting them in your Python code. `base_url` allows to push to a different `ntfy` server than the default `https://ntfy.sh`.
 2. `[notify_defaults]` with optional fields listed below, which will define default parameters used by `Notifier.notify(...)`. For instance you can set default `title` and `tags` for your code's `.notify(...)` calls and override them at specific locations with keyword arguments `.notify(title="Non-default title")`
    1. The behavior of the `title`, `priority`, `tags`, `click`, `attach`, `actions` and `icon` keys is described in the [`ntfy` docs](https://ntfy.sh/docs/publish/)
 
 ```ini
 # For Notifier(emails=..., topics=...)
 [notifier_init]
 topics = my-secret-topic-1, mysecrettopic2
 emails = you@foo.bar
+base_url = https://custom-ntfy-instance.io
 
 # For Notifier.notify(title=..., priority=..., etc.)
 [notify_defaults]
 title = Message from ntfy-wrapper
 priority = 0
 tags = fire
 click =
```

