# Comparing `tmp/burlap-0.9.98.tar.gz` & `tmp/burlap-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/burlap-0.9.98.tar", last modified: Tue May 17 17:27:46 2022, max compression
+gzip compressed data, was "dist/burlap-0.9.99.tar", last modified: Fri May 27 21:45:23 2022, max compression
```

## Comparing `burlap-0.9.98.tar` & `burlap-0.9.99.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/
--rw-r--r--   0 chris     (1000) chris     (1000)     1080 2019-06-18 16:05:45.000000 burlap-0.9.98/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)      162 2019-06-18 16:05:45.000000 burlap-0.9.98/MANIFEST.in
--rw-rw-r--   0 chris     (1000) chris     (1000)     6532 2022-05-17 17:27:46.000000 burlap-0.9.98/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4691 2020-04-24 03:01:07.000000 burlap-0.9.98/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/bin/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2689 2020-08-27 20:14:28.000000 burlap-0.9.98/bin/burlap-admin.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/
--rw-r--r--   0 chris     (1000) chris     (1000)    14662 2022-05-17 17:27:26.000000 burlap-0.9.98/burlap/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    26842 2020-10-27 13:55:01.000000 burlap-0.9.98/burlap/apache.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1864 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/avahi.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4811 2022-01-20 17:33:14.000000 burlap-0.9.98/burlap/aws.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1504 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/bluetooth.py
--rw-r--r--   0 chris     (1000) chris     (1000)    19709 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/buildbot.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5811 2021-03-24 05:14:09.000000 burlap-0.9.98/burlap/celery.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1826 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/cloudfront.py
--rw-r--r--   0 chris     (1000) chris     (1000)    94196 2021-05-14 00:56:47.000000 burlap-0.9.98/burlap/common.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1147 2021-07-28 01:19:08.000000 burlap-0.9.98/burlap/constants.py
--rw-r--r--   0 chris     (1000) chris     (1000)      397 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/context.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5582 2022-02-03 01:41:32.000000 burlap-0.9.98/burlap/cron.py
--rw-r--r--   0 chris     (1000) chris     (1000)    15135 2022-01-20 17:41:00.000000 burlap-0.9.98/burlap/db.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6985 2022-05-17 17:27:07.000000 burlap-0.9.98/burlap/deb.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10326 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/debug.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3114 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/decorators.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14317 2022-01-31 03:06:30.000000 burlap-0.9.98/burlap/deploy.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3263 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/disk.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    37405 2022-01-22 00:27:48.000000 burlap-0.9.98/burlap/dj.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4420 2021-09-21 17:08:14.000000 burlap-0.9.98/burlap/dns.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2956 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/elasticsearch.py
--rw-r--r--   0 chris     (1000) chris     (1000)       92 2020-01-09 18:02:15.000000 burlap-0.9.98/burlap/exceptions.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16437 2021-05-14 00:54:35.000000 burlap-0.9.98/burlap/files.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/fixtures/
--rw-rw-r--   0 chris     (1000) chris     (1000)      152 2021-11-11 22:30:31.000000 burlap-0.9.98/burlap/fixtures/requirements.txt
--rw-r--r--   0 chris     (1000) chris     (1000)    12857 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/git.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1626 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/gpsd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1002 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/group.py
--rw-r--r--   0 chris     (1000) chris     (1000)    17778 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/host.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3450 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/inadyn.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2321 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/ip.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10938 2020-07-29 18:24:10.000000 burlap-0.9.98/burlap/jirahelper.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1282 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/js.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1947 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/locale.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3139 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/mail.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2222 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/manifest.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1712 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/memcached.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6420 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/mongodb.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1494 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/motion.py
--rw-r--r--   0 chris     (1000) chris     (1000)    23289 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/mysql.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1476 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/network.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5926 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/networkmanager.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6512 2020-07-29 18:24:10.000000 burlap-0.9.98/burlap/notifier.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2133 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/ntp.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16326 2021-05-14 00:57:57.000000 burlap-0.9.98/burlap/packager.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2138 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/phantomjs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7579 2022-05-17 17:27:07.000000 burlap-0.9.98/burlap/pip.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    29430 2022-05-13 18:38:48.000000 burlap-0.9.98/burlap/postgresql.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10934 2022-04-04 19:09:51.000000 burlap-0.9.98/burlap/project.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3891 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/python_setuptools.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12466 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/rabbitmq.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3818 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/raid.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    23321 2022-05-17 17:27:07.000000 burlap-0.9.98/burlap/rpi.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5425 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/rpm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1401 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/rsync.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6714 2021-08-18 02:17:10.000000 burlap-0.9.98/burlap/s3.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2366 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/security.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4789 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/selenium.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3599 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/service.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1531 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/settings.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1591 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/shelf.py
--rw-r--r--   0 chris     (1000) chris     (1000)      523 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/snort.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4095 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/ssh.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5984 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/sslhelper.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9330 2021-12-08 02:17:11.000000 burlap-0.9.98/burlap/supervisor.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7315 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/system.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2369 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/systemd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4643 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tarball.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1299 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tasks.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/apache/
--rw-r--r--   0 chris     (1000) chris     (1000)       71 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/apache/apache_httpd.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)     1643 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/apache/apache_modevasive.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)     7477 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/apache/apache_modsecurity.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)      625 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/apache/apache_ports.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)     4053 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/apache/apache_site.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)      121 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/apache/maintenance.html.template
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/avahi/
--rw-r--r--   0 chris     (1000) chris     (1000)     1755 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/avahi/etc_avahi_avahi_daemon_conf
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/buildbot/
--rw-r--r--   0 chris     (1000) chris     (1000)      268 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/buildbot/check_buildbot.sh.template
--rw-r--r--   0 chris     (1000) chris     (1000)      318 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/buildbot/etc_crond_buildbot.template
--rw-r--r--   0 chris     (1000) chris     (1000)     1018 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/buildbot/supervisor.conf.template
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/burlap/
--rw-r--r--   0 chris     (1000) chris     (1000)     1025 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/burlap/all_settings.yaml.template
--rw-r--r--   0 chris     (1000) chris     (1000)      370 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/burlap/fabfile.py.template
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/burlap/gitignore.template
--rw-r--r--   0 chris     (1000) chris     (1000)      339 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/burlap/role_settings.yaml.template
--rw-r--r--   0 chris     (1000) chris     (1000)     1095 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/burlap/satchel.py.template
--rw-r--r--   0 chris     (1000) chris     (1000)      238 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/burlap/setup.bash.template
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/celery/
--rw-r--r--   0 chris     (1000) chris     (1000)      537 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/celery/celery_daemon.template.config
--rw-r--r--   0 chris     (1000) chris     (1000)     2309 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/celery/celery_daemon.template.init
--rw-r--r--   0 chris     (1000) chris     (1000)     1039 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/celery/celery_supervisor.template.conf
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/django/
--rw-r--r--   0 chris     (1000) chris     (1000)      655 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/django/django.template.wsgi
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/ec2monitor/
--rw-rw-r--   0 chris     (1000) chris     (1000)      336 2022-01-20 17:33:14.000000 burlap-0.9.98/burlap/templates/ec2monitor/etc_crond_ec2monitor
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/git/
--rw-r--r--   0 chris     (1000) chris     (1000)      477 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/git/post-checkout
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/inadyn/
--rw-r--r--   0 chris     (1000) chris     (1000)      470 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/inadyn/etc_default_inadyn.template
--rw-r--r--   0 chris     (1000) chris     (1000)      980 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/inadyn/etc_inadyn_conf.template
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/ip/
--rw-r--r--   0 chris     (1000) chris     (1000)      500 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/ip/ip_interfaces_dynamic.template
--rw-r--r--   0 chris     (1000) chris     (1000)      301 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/ip/ip_interfaces_static.template
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/iptables/
--rw-r--r--   0 chris     (1000) chris     (1000)     1033 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/iptables/iptables.template.rules
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/mongodb/
--rw-r--r--   0 chris     (1000) chris     (1000)      221 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/mongodb/etc_crond_mongomonitor
--rwxr-xr-x   0 chris     (1000) chris     (1000)      162 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/mongodb/mongomonitor
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/nm/
--rw-r--r--   0 chris     (1000) chris     (1000)      583 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/nm/check_networkmanager.sh
--rw-r--r--   0 chris     (1000) chris     (1000)      284 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/nm/etc_crond_check_networkmanager
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/notifier/
--rw-r--r--   0 chris     (1000) chris     (1000)      378 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/notifier/loginnotifier.template.sh
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/postfix/
--rw-r--r--   0 chris     (1000) chris     (1000)     1572 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/postfix/etc_postfix_main.cf
--rw-r--r--   0 chris     (1000) chris     (1000)       86 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/postfix/etc_postfix_sasl_sasl_passwd
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/postgresql/
--rw-r--r--   0 chris     (1000) chris     (1000)      474 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/postgresql/pg_hba.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)    23568 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/postgresql/postgresql-9.3.template.conf
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/rabbitmq/
--rw-r--r--   0 chris     (1000) chris     (1000)      354 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/rabbitmq/etc_crond_purge_mnesia.template
--rw-r--r--   0 chris     (1000) chris     (1000)      793 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/rabbitmq/purge_mnesia.sh.template
--rw-r--r--   0 chris     (1000) chris     (1000)      365 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/rabbitmq/rabbitmq.template.conf
--rw-r--r--   0 chris     (1000) chris     (1000)      112 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/rabbitmq/rabbitmq_cluster.template.config
--rw-r--r--   0 chris     (1000) chris     (1000)       32 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/rabbitmq/rabbitmq_doterlang.template.cookie
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/softwareraid/
--rw-r--r--   0 chris     (1000) chris     (1000)      327 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/softwareraid/wait_for_raid.sh
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/sshnice/
--rw-r--r--   0 chris     (1000) chris     (1000)      290 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/sshnice/etc_crond_sshnice
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/supervisor/
--rw-r--r--   0 chris     (1000) chris     (1000)     8537 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/supervisor/supervisor_daemon.template.config
--rw-r--r--   0 chris     (1000) chris     (1000)     4680 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/supervisor/supervisor_daemon.template.init
--rw-r--r--   0 chris     (1000) chris     (1000)     1216 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/supervisor/supervisor_daemon.template2.config
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/templates/unattendedupgrades/
--rw-r--r--   0 chris     (1000) chris     (1000)      349 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/unattendedupgrades/etc_apt_aptconfd_10periodic
--rw-r--r--   0 chris     (1000) chris     (1000)     2454 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/templates/unattendedupgrades/etc_apt_aptconfd_50unattended_upgrades
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/tests/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/tests/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5245 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/base.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap/tests/functional_tests/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/tests/functional_tests/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)      961 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/tests/functional_tests/base.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6905 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/conftest.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3670 2022-05-17 17:27:07.000000 burlap-0.9.98/burlap/tests/functional_tests/test_buildbot.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1578 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_common.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8047 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_deploy.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1835 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_git.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1576 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_js.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1505 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_locale.py
--rw-r--r--   0 chris     (1000) chris     (1000)      844 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_md5.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2630 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/functional_tests/test_mysql.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1994 2019-10-21 20:24:14.000000 burlap-0.9.98/burlap/tests/functional_tests/test_network.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5048 2019-10-22 22:51:26.000000 burlap-0.9.98/burlap/tests/functional_tests/test_selenium.py
--rw-r--r--   0 chris     (1000) chris     (1000)      501 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/tests/functional_tests/test_timezone.py
--rw-r--r--   0 chris     (1000) chris     (1000)      460 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/tests/functional_tests/test_users.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7520 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_apache.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12143 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_common.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1191 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_debug.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8624 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_dj.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1265 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_jirahelper.py
--rw-r--r--   0 chris     (1000) chris     (1000)      361 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_locale.py
--rw-r--r--   0 chris     (1000) chris     (1000)      683 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_manifest.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1713 2021-07-28 01:19:08.000000 burlap-0.9.98/burlap/tests/test_pip.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5928 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/tests/test_project.py
--rw-r--r--   0 chris     (1000) chris     (1000)      737 2019-06-18 16:05:45.000000 burlap-0.9.98/burlap/tests/test_service.py
--rw-r--r--   0 chris     (1000) chris     (1000)      644 2019-10-21 20:28:18.000000 burlap-0.9.98/burlap/tests/test_system.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2394 2019-10-21 20:33:52.000000 burlap-0.9.98/burlap/tests/test_vagrant_base_boxes.py
--rw-r--r--   0 chris     (1000) chris     (1000)      577 2019-10-22 18:47:02.000000 burlap-0.9.98/burlap/tests/test_vagrant_machines.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4928 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/trackers.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12008 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/user.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2357 2021-05-14 00:57:32.000000 burlap-0.9.98/burlap/utils.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9355 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/vagrant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8625 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/versioner.py
--rw-r--r--   0 chris     (1000) chris     (1000)      997 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/virtualbox.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14221 2020-08-27 20:14:28.000000 burlap-0.9.98/burlap/vm.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6532 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     5138 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2019-06-18 20:18:14.000000 burlap-0.9.98/burlap.egg-info/not-zip-safe
--rw-r--r--   0 chris     (1000) chris     (1000)      172 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        7 2022-05-17 17:27:46.000000 burlap-0.9.98/burlap.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      118 2021-05-14 02:13:01.000000 burlap-0.9.98/requirements-test.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-05-17 17:27:46.000000 burlap-0.9.98/setup.cfg
--rw-r--r--   0 chris     (1000) chris     (1000)     2680 2020-04-24 03:01:07.000000 burlap-0.9.98/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1080 2019-06-18 16:05:45.000000 burlap-0.9.99/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)      162 2019-06-18 16:05:45.000000 burlap-0.9.99/MANIFEST.in
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6532 2022-05-27 21:45:23.000000 burlap-0.9.99/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4691 2020-04-24 03:01:07.000000 burlap-0.9.99/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/bin/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2689 2020-08-27 20:14:28.000000 burlap-0.9.99/bin/burlap-admin.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/
+-rw-r--r--   0 chris     (1000) chris     (1000)    14662 2022-05-27 21:45:01.000000 burlap-0.9.99/burlap/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    26842 2020-10-27 13:55:01.000000 burlap-0.9.99/burlap/apache.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1864 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/avahi.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4811 2022-01-20 17:33:14.000000 burlap-0.9.99/burlap/aws.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1504 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/bluetooth.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    19882 2022-05-27 21:45:13.000000 burlap-0.9.99/burlap/buildbot.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5811 2021-03-24 05:14:09.000000 burlap-0.9.99/burlap/celery.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1826 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/cloudfront.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    94196 2021-05-14 00:56:47.000000 burlap-0.9.99/burlap/common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1147 2021-07-28 01:19:08.000000 burlap-0.9.99/burlap/constants.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      397 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/context.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5582 2022-02-03 01:41:32.000000 burlap-0.9.99/burlap/cron.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    15135 2022-01-20 17:41:00.000000 burlap-0.9.99/burlap/db.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6985 2022-05-17 17:27:07.000000 burlap-0.9.99/burlap/deb.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10326 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/debug.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3114 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/decorators.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    14317 2022-01-31 03:06:30.000000 burlap-0.9.99/burlap/deploy.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3263 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/disk.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    37405 2022-01-22 00:27:48.000000 burlap-0.9.99/burlap/dj.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4420 2021-09-21 17:08:14.000000 burlap-0.9.99/burlap/dns.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2956 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/elasticsearch.py
+-rw-r--r--   0 chris     (1000) chris     (1000)       92 2020-01-09 18:02:15.000000 burlap-0.9.99/burlap/exceptions.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    16437 2021-05-14 00:54:35.000000 burlap-0.9.99/burlap/files.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/fixtures/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      152 2021-11-11 22:30:31.000000 burlap-0.9.99/burlap/fixtures/requirements.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)    12857 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/git.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1626 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/gpsd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1002 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/group.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    17778 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/host.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3450 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/inadyn.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2321 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/ip.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10938 2020-07-29 18:24:10.000000 burlap-0.9.99/burlap/jirahelper.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1282 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/js.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1947 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/locale.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3139 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/mail.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2222 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/manifest.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1712 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/memcached.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6420 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/mongodb.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1494 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/motion.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    23289 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/mysql.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1476 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/network.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5926 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/networkmanager.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6512 2020-07-29 18:24:10.000000 burlap-0.9.99/burlap/notifier.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2133 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/ntp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    16326 2021-05-14 00:57:57.000000 burlap-0.9.99/burlap/packager.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2138 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/phantomjs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7579 2022-05-17 17:27:07.000000 burlap-0.9.99/burlap/pip.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    29430 2022-05-13 18:38:48.000000 burlap-0.9.99/burlap/postgresql.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10934 2022-04-04 19:09:51.000000 burlap-0.9.99/burlap/project.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3891 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/python_setuptools.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12466 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/rabbitmq.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3818 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/raid.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23321 2022-05-17 17:27:07.000000 burlap-0.9.99/burlap/rpi.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5425 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/rpm.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1401 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/rsync.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6714 2021-08-18 02:17:10.000000 burlap-0.9.99/burlap/s3.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2366 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/security.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4789 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/selenium.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3599 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/service.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1531 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/settings.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1591 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/shelf.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      523 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/snort.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4095 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/ssh.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5984 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/sslhelper.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9330 2021-12-08 02:17:11.000000 burlap-0.9.99/burlap/supervisor.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7315 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/system.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2369 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/systemd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4643 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tarball.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1299 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tasks.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/apache/
+-rw-r--r--   0 chris     (1000) chris     (1000)       71 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/apache/apache_httpd.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)     1643 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/apache/apache_modevasive.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)     7477 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/apache/apache_modsecurity.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)      625 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/apache/apache_ports.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)     4053 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/apache/apache_site.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)      121 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/apache/maintenance.html.template
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/avahi/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1755 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/avahi/etc_avahi_avahi_daemon_conf
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/buildbot/
+-rw-r--r--   0 chris     (1000) chris     (1000)      268 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/buildbot/check_buildbot.sh.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      318 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/buildbot/etc_crond_buildbot.template
+-rw-r--r--   0 chris     (1000) chris     (1000)     1018 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/buildbot/supervisor.conf.template
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/burlap/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1025 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/burlap/all_settings.yaml.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      370 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/burlap/fabfile.py.template
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/burlap/gitignore.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      339 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/burlap/role_settings.yaml.template
+-rw-r--r--   0 chris     (1000) chris     (1000)     1095 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/burlap/satchel.py.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      238 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/burlap/setup.bash.template
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/celery/
+-rw-r--r--   0 chris     (1000) chris     (1000)      537 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/celery/celery_daemon.template.config
+-rw-r--r--   0 chris     (1000) chris     (1000)     2309 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/celery/celery_daemon.template.init
+-rw-r--r--   0 chris     (1000) chris     (1000)     1039 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/celery/celery_supervisor.template.conf
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/django/
+-rw-r--r--   0 chris     (1000) chris     (1000)      655 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/django/django.template.wsgi
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/ec2monitor/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      336 2022-01-20 17:33:14.000000 burlap-0.9.99/burlap/templates/ec2monitor/etc_crond_ec2monitor
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/git/
+-rw-r--r--   0 chris     (1000) chris     (1000)      477 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/git/post-checkout
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/inadyn/
+-rw-r--r--   0 chris     (1000) chris     (1000)      470 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/inadyn/etc_default_inadyn.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      980 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/inadyn/etc_inadyn_conf.template
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/ip/
+-rw-r--r--   0 chris     (1000) chris     (1000)      500 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/ip/ip_interfaces_dynamic.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      301 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/ip/ip_interfaces_static.template
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/iptables/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1033 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/iptables/iptables.template.rules
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/mongodb/
+-rw-r--r--   0 chris     (1000) chris     (1000)      221 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/mongodb/etc_crond_mongomonitor
+-rwxr-xr-x   0 chris     (1000) chris     (1000)      162 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/mongodb/mongomonitor
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/nm/
+-rw-r--r--   0 chris     (1000) chris     (1000)      583 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/nm/check_networkmanager.sh
+-rw-r--r--   0 chris     (1000) chris     (1000)      284 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/nm/etc_crond_check_networkmanager
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/notifier/
+-rw-r--r--   0 chris     (1000) chris     (1000)      378 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/notifier/loginnotifier.template.sh
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/postfix/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1572 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/postfix/etc_postfix_main.cf
+-rw-r--r--   0 chris     (1000) chris     (1000)       86 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/postfix/etc_postfix_sasl_sasl_passwd
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/postgresql/
+-rw-r--r--   0 chris     (1000) chris     (1000)      474 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/postgresql/pg_hba.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)    23568 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/postgresql/postgresql-9.3.template.conf
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/rabbitmq/
+-rw-r--r--   0 chris     (1000) chris     (1000)      354 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/rabbitmq/etc_crond_purge_mnesia.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      793 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/rabbitmq/purge_mnesia.sh.template
+-rw-r--r--   0 chris     (1000) chris     (1000)      365 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/rabbitmq/rabbitmq.template.conf
+-rw-r--r--   0 chris     (1000) chris     (1000)      112 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/rabbitmq/rabbitmq_cluster.template.config
+-rw-r--r--   0 chris     (1000) chris     (1000)       32 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/rabbitmq/rabbitmq_doterlang.template.cookie
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/softwareraid/
+-rw-r--r--   0 chris     (1000) chris     (1000)      327 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/softwareraid/wait_for_raid.sh
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/sshnice/
+-rw-r--r--   0 chris     (1000) chris     (1000)      290 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/sshnice/etc_crond_sshnice
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/supervisor/
+-rw-r--r--   0 chris     (1000) chris     (1000)     8537 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/supervisor/supervisor_daemon.template.config
+-rw-r--r--   0 chris     (1000) chris     (1000)     4680 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/supervisor/supervisor_daemon.template.init
+-rw-r--r--   0 chris     (1000) chris     (1000)     1216 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/supervisor/supervisor_daemon.template2.config
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/templates/unattendedupgrades/
+-rw-r--r--   0 chris     (1000) chris     (1000)      349 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/unattendedupgrades/etc_apt_aptconfd_10periodic
+-rw-r--r--   0 chris     (1000) chris     (1000)     2454 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/templates/unattendedupgrades/etc_apt_aptconfd_50unattended_upgrades
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/tests/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/tests/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5245 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/base.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap/tests/functional_tests/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/tests/functional_tests/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      961 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/tests/functional_tests/base.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6905 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/conftest.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3670 2022-05-17 17:27:07.000000 burlap-0.9.99/burlap/tests/functional_tests/test_buildbot.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1578 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_common.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8047 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_deploy.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1835 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_git.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1576 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_js.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1505 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_locale.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      844 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_md5.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2630 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/functional_tests/test_mysql.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1994 2019-10-21 20:24:14.000000 burlap-0.9.99/burlap/tests/functional_tests/test_network.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5048 2019-10-22 22:51:26.000000 burlap-0.9.99/burlap/tests/functional_tests/test_selenium.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      501 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/tests/functional_tests/test_timezone.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      460 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/tests/functional_tests/test_users.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7520 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_apache.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12143 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_common.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1191 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_debug.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8624 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_dj.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1265 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_jirahelper.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      361 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_locale.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      683 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_manifest.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1713 2021-07-28 01:19:08.000000 burlap-0.9.99/burlap/tests/test_pip.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5928 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/tests/test_project.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      737 2019-06-18 16:05:45.000000 burlap-0.9.99/burlap/tests/test_service.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      644 2019-10-21 20:28:18.000000 burlap-0.9.99/burlap/tests/test_system.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2394 2019-10-21 20:33:52.000000 burlap-0.9.99/burlap/tests/test_vagrant_base_boxes.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      577 2019-10-22 18:47:02.000000 burlap-0.9.99/burlap/tests/test_vagrant_machines.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4928 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/trackers.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12008 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/user.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2357 2021-05-14 00:57:32.000000 burlap-0.9.99/burlap/utils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9355 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/vagrant.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8625 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/versioner.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      997 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/virtualbox.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    14221 2020-08-27 20:14:28.000000 burlap-0.9.99/burlap/vm.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-05-27 21:45:23.000000 burlap-0.9.99/burlap.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6532 2022-05-27 21:45:22.000000 burlap-0.9.99/burlap.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     5138 2022-05-27 21:45:22.000000 burlap-0.9.99/burlap.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2022-05-27 21:45:22.000000 burlap-0.9.99/burlap.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2019-06-18 20:18:14.000000 burlap-0.9.99/burlap.egg-info/not-zip-safe
+-rw-r--r--   0 chris     (1000) chris     (1000)      172 2022-05-27 21:45:22.000000 burlap-0.9.99/burlap.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        7 2022-05-27 21:45:22.000000 burlap-0.9.99/burlap.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      118 2021-05-14 02:13:01.000000 burlap-0.9.99/requirements-test.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-05-27 21:45:23.000000 burlap-0.9.99/setup.cfg
+-rw-r--r--   0 chris     (1000) chris     (1000)     2680 2020-04-24 03:01:07.000000 burlap-0.9.99/setup.py
```

### Comparing `burlap-0.9.98/LICENSE` & `burlap-0.9.99/LICENSE`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/PKG-INFO` & `burlap-0.9.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burlap
-Version: 0.9.98
+Version: 0.9.99
 Summary: Fabric commands for simplifying server deployments
 Home-page: https://gitlab.com/chrisspen/burlap
 Author: Chris Spencer
 Author-email: chrisspen@gmail.com
 License: MIT
 Description: Burlap - configuration management designed for simplicity and speed
         ===================================================================
```

### Comparing `burlap-0.9.98/README.md` & `burlap-0.9.99/README.md`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/bin/burlap-admin.py` & `burlap-0.9.99/bin/burlap-admin.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/__init__.py` & `burlap-0.9.99/burlap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 try:
     from . import debug
 except (ImportError, NameError) as e:
     print('Unable to initialize debug: %s' % e, file=sys.stderr)
     debug = None
 
-VERSION = (0, 9, 98)
+VERSION = (0, 9, 99)
 __version__ = '.'.join(map(str, VERSION))
 
 burlap_populate_stack = int(os.environ.get('BURLAP_POPULATE_STACK', 1))
 no_load = int(os.environ.get('BURLAP_NO_LOAD', 0))
 
 # Show virtually all logging messages by default.
 default_loglevel = logging.getLevelName(os.environ.get('LOGLEVEL', 'INFO'))
```

### Comparing `burlap-0.9.98/burlap/apache.py` & `burlap-0.9.99/burlap/apache.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/avahi.py` & `burlap-0.9.99/burlap/avahi.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/aws.py` & `burlap-0.9.99/burlap/aws.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/bluetooth.py` & `burlap-0.9.99/burlap/bluetooth.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/buildbot.py` & `burlap-0.9.99/burlap/buildbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
         self.env.project_dir = '/usr/local/myproject'
         self.env.virtualenv_dir = '/usr/local/myproject/.env'
         self.env.home_dir = '/var/lib/{bb_user}'
         self.env.src_dir = 'src/buildbot'
 
         self.env.ssh_bin = '{home_dir}/bin'
         self.env.ssh_dir = '{home_dir}/.ssh'
-        self.env.ssh_private_key = None # should be a *.pem file
-        self.env.ssh_public_key = None # should be a *.pub file
+        self.env.ssh_private_key = 'roles/{ROLE}/id_ed25519' # Relative path to local copy of SSH private key
+        self.env.ssh_public_key = 'roles/{ROLE}/id_ed25519.pub' # Relative path to local copy of SSH public key
+        self.env.private_remote_path = '{ssh_dir}/id_ed25519' # Absolute path to remote copy of SSH private key
+        self.env.public_remote_path = '{ssh_dir}/id_ed25519.pub' # Absolute path to remote copy of SSH public key
 
         # Must match the main user, or otherwise we get rsync errors.
         self.env.user = 'ubuntu'
         self.env.group = 'ubuntu'
 
         self.env.bb_user = 'buildbot'
         self.env.bb_group = 'buildbot'
@@ -385,21 +387,20 @@
         #user.create(self.env.bb_user, self.env.bb_group)
 
     def deploy_pre_run(self):
         self.check_ok()
 
     @task
     def configure_ssh_key(self):
+        """
+        Install the read-only SSH key on the server, so it can access private git repos.
+        """
         r = self.local_renderer
-        r.env.private_remote_path = '{ssh_dir}/id_rsa'
-        r.env.public_remote_path = '{ssh_dir}/id_rsa.pub'
         if r.env.use_ssh_key:
             #https://www.cyberciti.biz/faq/how-to-set-up-ssh-keys-on-linux-unix/
-            assert r.env.ssh_private_key, 'No SSH private key specified!'
-            assert r.env.ssh_public_key, 'No SSH public key specified!'
             r.sudo('mkdir -p {ssh_dir}')
             r.put(local_path=r.env.ssh_private_key, remote_path=r.env.private_remote_path, use_sudo=True)
             r.put(local_path=r.env.ssh_public_key, remote_path=r.env.public_remote_path, use_sudo=True)
             r.sudo('chown -R {bb_user}:{bb_group} {ssh_dir}')
             r.sudo('chmod -R 0770 {ssh_dir}')
             r.sudo('chmod -R 0600 {ssh_dir}/*') # SSH keys must use restrictive permissions.
         else:
```

### Comparing `burlap-0.9.98/burlap/celery.py` & `burlap-0.9.99/burlap/celery.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/cloudfront.py` & `burlap-0.9.99/burlap/cloudfront.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/common.py` & `burlap-0.9.99/burlap/common.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/constants.py` & `burlap-0.9.99/burlap/constants.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/cron.py` & `burlap-0.9.99/burlap/cron.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/db.py` & `burlap-0.9.99/burlap/db.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/deb.py` & `burlap-0.9.99/burlap/deb.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/debug.py` & `burlap-0.9.99/burlap/debug.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/decorators.py` & `burlap-0.9.99/burlap/decorators.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/deploy.py` & `burlap-0.9.99/burlap/deploy.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/disk.py` & `burlap-0.9.99/burlap/disk.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/dj.py` & `burlap-0.9.99/burlap/dj.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/dns.py` & `burlap-0.9.99/burlap/dns.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/elasticsearch.py` & `burlap-0.9.99/burlap/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/files.py` & `burlap-0.9.99/burlap/files.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/git.py` & `burlap-0.9.99/burlap/git.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/gpsd.py` & `burlap-0.9.99/burlap/gpsd.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/group.py` & `burlap-0.9.99/burlap/group.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/host.py` & `burlap-0.9.99/burlap/host.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/inadyn.py` & `burlap-0.9.99/burlap/inadyn.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/ip.py` & `burlap-0.9.99/burlap/ip.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/jirahelper.py` & `burlap-0.9.99/burlap/jirahelper.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/js.py` & `burlap-0.9.99/burlap/js.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/locale.py` & `burlap-0.9.99/burlap/locale.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/mail.py` & `burlap-0.9.99/burlap/mail.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/manifest.py` & `burlap-0.9.99/burlap/manifest.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/memcached.py` & `burlap-0.9.99/burlap/memcached.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/mongodb.py` & `burlap-0.9.99/burlap/mongodb.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/motion.py` & `burlap-0.9.99/burlap/motion.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/mysql.py` & `burlap-0.9.99/burlap/mysql.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/network.py` & `burlap-0.9.99/burlap/network.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/networkmanager.py` & `burlap-0.9.99/burlap/networkmanager.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/notifier.py` & `burlap-0.9.99/burlap/notifier.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/ntp.py` & `burlap-0.9.99/burlap/ntp.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/packager.py` & `burlap-0.9.99/burlap/packager.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/phantomjs.py` & `burlap-0.9.99/burlap/phantomjs.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/pip.py` & `burlap-0.9.99/burlap/pip.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/postgresql.py` & `burlap-0.9.99/burlap/postgresql.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/project.py` & `burlap-0.9.99/burlap/project.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/python_setuptools.py` & `burlap-0.9.99/burlap/python_setuptools.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/rabbitmq.py` & `burlap-0.9.99/burlap/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/raid.py` & `burlap-0.9.99/burlap/raid.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/rpi.py` & `burlap-0.9.99/burlap/rpi.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/rpm.py` & `burlap-0.9.99/burlap/rpm.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/rsync.py` & `burlap-0.9.99/burlap/rsync.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/s3.py` & `burlap-0.9.99/burlap/s3.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/security.py` & `burlap-0.9.99/burlap/security.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/selenium.py` & `burlap-0.9.99/burlap/selenium.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/service.py` & `burlap-0.9.99/burlap/service.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/settings.py` & `burlap-0.9.99/burlap/settings.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/shelf.py` & `burlap-0.9.99/burlap/shelf.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/snort.py` & `burlap-0.9.99/burlap/snort.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/ssh.py` & `burlap-0.9.99/burlap/ssh.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/sslhelper.py` & `burlap-0.9.99/burlap/sslhelper.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/supervisor.py` & `burlap-0.9.99/burlap/supervisor.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/system.py` & `burlap-0.9.99/burlap/system.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/systemd.py` & `burlap-0.9.99/burlap/systemd.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tarball.py` & `burlap-0.9.99/burlap/tarball.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tasks.py` & `burlap-0.9.99/burlap/tasks.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/apache/apache_modevasive.template.conf` & `burlap-0.9.99/burlap/templates/apache/apache_modevasive.template.conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/apache/apache_modsecurity.template.conf` & `burlap-0.9.99/burlap/templates/apache/apache_modsecurity.template.conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/apache/apache_ports.template.conf` & `burlap-0.9.99/burlap/templates/apache/apache_ports.template.conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/apache/apache_site.template.conf` & `burlap-0.9.99/burlap/templates/apache/apache_site.template.conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/avahi/etc_avahi_avahi_daemon_conf` & `burlap-0.9.99/burlap/templates/avahi/etc_avahi_avahi_daemon_conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/buildbot/supervisor.conf.template` & `burlap-0.9.99/burlap/templates/buildbot/supervisor.conf.template`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/burlap/all_settings.yaml.template` & `burlap-0.9.99/burlap/templates/burlap/all_settings.yaml.template`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/burlap/satchel.py.template` & `burlap-0.9.99/burlap/templates/burlap/satchel.py.template`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/celery/celery_daemon.template.config` & `burlap-0.9.99/burlap/templates/celery/celery_daemon.template.config`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/celery/celery_daemon.template.init` & `burlap-0.9.99/burlap/templates/celery/celery_daemon.template.init`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/celery/celery_supervisor.template.conf` & `burlap-0.9.99/burlap/templates/celery/celery_supervisor.template.conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/django/django.template.wsgi` & `burlap-0.9.99/burlap/templates/django/django.template.wsgi`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/inadyn/etc_inadyn_conf.template` & `burlap-0.9.99/burlap/templates/inadyn/etc_inadyn_conf.template`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/iptables/iptables.template.rules` & `burlap-0.9.99/burlap/templates/iptables/iptables.template.rules`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/nm/check_networkmanager.sh` & `burlap-0.9.99/burlap/templates/nm/check_networkmanager.sh`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/postfix/etc_postfix_main.cf` & `burlap-0.9.99/burlap/templates/postfix/etc_postfix_main.cf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/postgresql/postgresql-9.3.template.conf` & `burlap-0.9.99/burlap/templates/postgresql/postgresql-9.3.template.conf`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/rabbitmq/purge_mnesia.sh.template` & `burlap-0.9.99/burlap/templates/rabbitmq/purge_mnesia.sh.template`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/supervisor/supervisor_daemon.template.config` & `burlap-0.9.99/burlap/templates/supervisor/supervisor_daemon.template.config`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/supervisor/supervisor_daemon.template.init` & `burlap-0.9.99/burlap/templates/supervisor/supervisor_daemon.template.init`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/supervisor/supervisor_daemon.template2.config` & `burlap-0.9.99/burlap/templates/supervisor/supervisor_daemon.template2.config`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/templates/unattendedupgrades/etc_apt_aptconfd_50unattended_upgrades` & `burlap-0.9.99/burlap/templates/unattendedupgrades/etc_apt_aptconfd_50unattended_upgrades`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/base.py` & `burlap-0.9.99/burlap/tests/base.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/base.py` & `burlap-0.9.99/burlap/tests/functional_tests/base.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/conftest.py` & `burlap-0.9.99/burlap/tests/functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_buildbot.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_buildbot.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_common.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_common.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_deploy.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_git.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_git.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_js.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_js.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_locale.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_md5.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_md5.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_mysql.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_network.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_network.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/functional_tests/test_selenium.py` & `burlap-0.9.99/burlap/tests/functional_tests/test_selenium.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_apache.py` & `burlap-0.9.99/burlap/tests/test_apache.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_common.py` & `burlap-0.9.99/burlap/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_debug.py` & `burlap-0.9.99/burlap/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_dj.py` & `burlap-0.9.99/burlap/tests/test_dj.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_jirahelper.py` & `burlap-0.9.99/burlap/tests/test_jirahelper.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_manifest.py` & `burlap-0.9.99/burlap/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_pip.py` & `burlap-0.9.99/burlap/tests/test_pip.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_project.py` & `burlap-0.9.99/burlap/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_service.py` & `burlap-0.9.99/burlap/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_system.py` & `burlap-0.9.99/burlap/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_vagrant_base_boxes.py` & `burlap-0.9.99/burlap/tests/test_vagrant_base_boxes.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/tests/test_vagrant_machines.py` & `burlap-0.9.99/burlap/tests/test_vagrant_machines.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/trackers.py` & `burlap-0.9.99/burlap/trackers.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/user.py` & `burlap-0.9.99/burlap/user.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/utils.py` & `burlap-0.9.99/burlap/utils.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/vagrant.py` & `burlap-0.9.99/burlap/vagrant.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/versioner.py` & `burlap-0.9.99/burlap/versioner.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/virtualbox.py` & `burlap-0.9.99/burlap/virtualbox.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap/vm.py` & `burlap-0.9.99/burlap/vm.py`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/burlap.egg-info/PKG-INFO` & `burlap-0.9.99/burlap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burlap
-Version: 0.9.98
+Version: 0.9.99
 Summary: Fabric commands for simplifying server deployments
 Home-page: https://gitlab.com/chrisspen/burlap
 Author: Chris Spencer
 Author-email: chrisspen@gmail.com
 License: MIT
 Description: Burlap - configuration management designed for simplicity and speed
         ===================================================================
```

### Comparing `burlap-0.9.98/burlap.egg-info/SOURCES.txt` & `burlap-0.9.99/burlap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burlap-0.9.98/setup.py` & `burlap-0.9.99/setup.py`

 * *Files identical despite different names*

