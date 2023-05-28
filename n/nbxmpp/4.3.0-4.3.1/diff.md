# Comparing `tmp/nbxmpp-4.3.0.tar.gz` & `tmp/nbxmpp-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbxmpp-4.3.0.tar", last modified: Fri May 26 16:39:21 2023, max compression
+gzip compressed data, was "nbxmpp-4.3.1.tar", last modified: Sun May 28 21:20:13 2023, max compression
```

## Comparing `nbxmpp-4.3.0.tar` & `nbxmpp-4.3.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.357421 nbxmpp-4.3.0/
--rw-rw-rw-   0 worker    (1000) worker    (1000)    35147 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/COPYING
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8171 2023-05-26 16:37:09.000000 nbxmpp-4.3.0/ChangeLog
--rw-rw-rw-   0 worker    (1000) worker    (1000)       91 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/MANIFEST.in
--rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-05-26 16:39:21.357421 nbxmpp-4.3.0/PKG-INFO
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1135 2023-01-23 23:24:27.000000 nbxmpp-4.3.0/README.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.269413 nbxmpp-4.3.0/nbxmpp/
--rw-rw-rw-   0 worker    (1000) worker    (1000)      138 2023-05-26 16:37:09.000000 nbxmpp-4.3.0/nbxmpp/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8454 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/addresses.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1961 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/c14n.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    29929 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/client.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4447 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/connection.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14689 2023-05-21 07:37:52.000000 nbxmpp-4.3.0/nbxmpp/const.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    19830 2023-02-03 15:54:25.000000 nbxmpp-4.3.0/nbxmpp/dispatcher.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4962 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/errors.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      820 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/exceptions.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    18944 2023-05-21 17:24:50.000000 nbxmpp-4.3.0/nbxmpp/http.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    18504 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/idlequeue.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.349420 nbxmpp-4.3.0/nbxmpp/modules/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3692 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/activity.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6961 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/adhoc.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3618 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/annotations.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1706 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/attention.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1469 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/base.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2496 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/bits_of_binary.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5103 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/blocking.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.349420 nbxmpp-4.3.0/nbxmpp/modules/bookmarks/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/bookmarks/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4130 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/bookmarks/native_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3379 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/bookmarks/pep_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1990 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/bookmarks/private_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5394 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/bookmarks/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1945 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/captcha.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1984 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/chat_markers.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2009 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/chatstates.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1847 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/correction.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    20214 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/dataforms.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6166 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/date_and_time.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4020 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/delay.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1980 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/delimiter.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4612 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/discovery.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1740 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/eme.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3837 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/entity_caps.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3983 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/entity_time.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2011 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/http_auth.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2899 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/http_upload.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5934 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/ibb.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1875 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/idle.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2101 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/iq.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3286 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/last_activity.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2888 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/location.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6373 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/mam.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4265 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/message.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4348 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/misc.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3099 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/mood.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.349420 nbxmpp-4.3.0/nbxmpp/modules/muc/
--rw-rw-rw-   0 worker    (1000) worker    (1000)       21 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/muc/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3478 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/muc/moderation.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    20848 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/muc/muc.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5726 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/muc/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7370 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/muclumbus.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4308 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/nickname.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    15721 2023-05-10 18:13:15.000000 nbxmpp-4.3.0/nbxmpp/modules/omemo.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1669 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/oob.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    13348 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/openpgp.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2180 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/pgplegacy.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1916 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/ping.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5368 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/presence.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14592 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/pubsub.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2275 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/reactions.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2986 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/receipts.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.353420 nbxmpp-4.3.0/nbxmpp/modules/register/
--rw-rw-rw-   0 worker    (1000) worker    (1000)       31 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/register/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3456 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/register/register.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4233 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/register/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3210 2023-02-03 15:54:25.000000 nbxmpp-4.3.0/nbxmpp/modules/replies.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     5512 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/roster.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1846 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/rsm.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4789 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/security_labels.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3829 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/software_version.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2965 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/tune.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    10856 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/user_avatar.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2558 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    31943 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/vcard4.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2214 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/vcard_avatar.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4366 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/modules/vcard_temp.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8820 2023-02-03 15:54:25.000000 nbxmpp-4.3.0/nbxmpp/namespaces.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    28667 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/old_dispatcher.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3549 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/plugin.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      499 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/precis.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    76385 2023-04-21 14:56:16.000000 nbxmpp-4.3.0/nbxmpp/protocol.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/py.typed
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14968 2023-04-23 13:45:46.000000 nbxmpp-4.3.0/nbxmpp/sasl.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    27907 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/simplexml.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    11907 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/smacks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8157 2023-02-05 14:55:00.000000 nbxmpp-4.3.0/nbxmpp/stringprep.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    34441 2023-05-10 18:13:15.000000 nbxmpp-4.3.0/nbxmpp/structs.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    11501 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/task.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    14807 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/tcp.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.353420 nbxmpp-4.3.0/nbxmpp/third_party/
--rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/third_party/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8903 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/third_party/hsluv.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      118 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/types.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)    15519 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     6386 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/nbxmpp/websocket.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1691 2023-04-21 14:56:16.000000 nbxmpp-4.3.0/nbxmpp/xmppiri.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.273413 nbxmpp-4.3.0/nbxmpp.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-05-26 16:39:20.000000 nbxmpp-4.3.0/nbxmpp.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     3241 2023-05-26 16:39:20.000000 nbxmpp-4.3.0/nbxmpp.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-05-26 16:39:20.000000 nbxmpp-4.3.0/nbxmpp.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       69 2023-05-26 16:39:20.000000 nbxmpp-4.3.0/nbxmpp.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        7 2023-05-26 16:39:20.000000 nbxmpp-4.3.0/nbxmpp.egg-info/top_level.txt
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1120 2023-01-23 23:24:27.000000 nbxmpp-4.3.0/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)       38 2023-05-26 16:39:21.357421 nbxmpp-4.3.0/setup.cfg
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.353420 nbxmpp-4.3.0/test/
--rw-rw-rw-   0 worker    (1000) worker    (1000)      116 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/__init__.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.353420 nbxmpp-4.3.0/test/lib/
--rw-rw-rw-   0 worker    (1000) worker    (1000)      837 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/lib/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      104 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/lib/const.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)      564 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/lib/util.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2706 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/lib/xmpp_mocks.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-26 16:39:21.357421 nbxmpp-4.3.0/test/unit/
--rw-rw-rw-   0 worker    (1000) worker    (1000)       54 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/__init__.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1975 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_activity.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2375 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_avatar.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4471 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_bookmarks.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4209 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_datetime_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1013 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_delay_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     8758 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_entity_caps.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1411 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_error_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7598 2023-05-19 07:16:33.000000 nbxmpp-4.3.0/test/unit/test_http.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7296 2023-04-21 14:56:16.000000 nbxmpp-4.3.0/test/unit/test_jid_parsing.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4360 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_location.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1724 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_mood.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1241 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_muclumbus.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     3159 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_pubsub.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     4555 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_reactions.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     1177 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_sasl_scram.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     7729 2023-02-05 14:55:00.000000 nbxmpp-4.3.0/test/unit/test_stringprep.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2279 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_tune.py
--rw-rw-rw-   0 worker    (1000) worker    (1000)     2389 2022-12-31 20:57:12.000000 nbxmpp-4.3.0/test/unit/test_xml_vulnerability.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    35147 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/COPYING
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8302 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/ChangeLog
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       91 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/MANIFEST.in
+-rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/PKG-INFO
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1135 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/README.md
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.251864 nbxmpp-4.3.1/nbxmpp/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      138 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/nbxmpp/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8454 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/addresses.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1961 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/c14n.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    29929 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/client.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4447 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/connection.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14689 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/const.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    19830 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/dispatcher.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4962 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/errors.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      820 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/exceptions.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    19012 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/nbxmpp/http.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    18504 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/idlequeue.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.271866 nbxmpp-4.3.1/nbxmpp/modules/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3692 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/activity.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6961 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/adhoc.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3618 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/annotations.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1706 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/attention.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1469 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/base.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2496 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bits_of_binary.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5103 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/blocking.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.275866 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4130 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/native_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3379 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/pep_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1990 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/private_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5394 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/bookmarks/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1945 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/captcha.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1984 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/chat_markers.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2009 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/chatstates.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1847 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/correction.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    20214 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/dataforms.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6166 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/date_and_time.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4020 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/delay.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1980 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/delimiter.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4612 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/discovery.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1740 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/eme.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3837 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/entity_caps.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3983 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/entity_time.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2011 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/http_auth.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2899 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/http_upload.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5934 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/ibb.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1875 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/idle.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2101 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/iq.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3286 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/last_activity.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2888 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/location.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6373 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/mam.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4265 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/message.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4348 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/misc.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3099 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/mood.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.275866 nbxmpp-4.3.1/nbxmpp/modules/muc/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       21 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3478 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/moderation.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    20848 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/muc.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5726 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muc/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     7370 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/muclumbus.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4308 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/nickname.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    15721 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/modules/omemo.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1669 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/oob.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    13348 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/openpgp.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2180 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/pgplegacy.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1916 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/ping.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5368 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/presence.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14592 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/pubsub.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2275 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/reactions.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2986 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/receipts.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/nbxmpp/modules/register/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       31 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/register/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3456 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/register/register.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4233 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/register/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3210 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/modules/replies.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     5512 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/roster.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1846 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/rsm.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4789 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/security_labels.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3829 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/software_version.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2965 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/tune.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    10856 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/user_avatar.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2558 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    31943 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/vcard4.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2214 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/vcard_avatar.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4366 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/modules/vcard_temp.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8820 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/namespaces.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    28667 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/old_dispatcher.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3549 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/plugin.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      499 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/precis.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    76385 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/protocol.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/py.typed
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14968 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/sasl.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    27907 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/simplexml.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    11907 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/smacks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8157 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/nbxmpp/stringprep.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    34441 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/structs.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    11501 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/task.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    14807 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/tcp.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/nbxmpp/third_party/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)        0 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/third_party/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8903 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/third_party/hsluv.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      118 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/types.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)    15519 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/nbxmpp/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     6873 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/nbxmpp/websocket.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1691 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/nbxmpp/xmppiri.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.255864 nbxmpp-4.3.1/nbxmpp.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1587 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     3241 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       69 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        7 2023-05-28 21:20:13.000000 nbxmpp-4.3.1/nbxmpp.egg-info/top_level.txt
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1120 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)       38 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/setup.cfg
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/test/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      116 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/__init__.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.279867 nbxmpp-4.3.1/test/lib/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      837 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/lib/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)      104 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/lib/const.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1322 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/test/lib/util.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2706 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/lib/xmpp_mocks.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-05-28 21:20:13.291868 nbxmpp-4.3.1/test/unit/
+-rw-rw-rw-   0 worker    (1000) worker    (1000)       54 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/__init__.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1975 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_activity.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2375 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_avatar.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4471 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_bookmarks.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4209 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_datetime_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1013 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_delay_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8758 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_entity_caps.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1411 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_error_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     8433 2023-05-28 21:18:48.000000 nbxmpp-4.3.1/test/unit/test_http.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     7296 2023-05-26 16:38:00.000000 nbxmpp-4.3.1/test/unit/test_jid_parsing.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4360 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_location.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1724 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_mood.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1241 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_muclumbus.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     3159 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_pubsub.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     4555 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_reactions.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     1177 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_sasl_scram.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     7729 2023-02-05 16:24:20.000000 nbxmpp-4.3.1/test/unit/test_stringprep.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2279 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_tune.py
+-rw-rw-rw-   0 worker    (1000) worker    (1000)     2389 2023-01-01 21:21:54.000000 nbxmpp-4.3.1/test/unit/test_xml_vulnerability.py
```

### Comparing `nbxmpp-4.3.0/COPYING` & `nbxmpp-4.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/ChangeLog` & `nbxmpp-4.3.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+nbxmpp 4.3.1 (28 May 2023)
+
+  Bug Fixes
+
+  * HTTP: Abort correctly on content overflow
+  * Websocket: Always set peer certificate
+
 nbxmpp 4.3.0 (21 May 2023)
 
   New
 
   * Add option to force http1
   * Add method to generate XMPP IRIs
```

### Comparing `nbxmpp-4.3.0/PKG-INFO` & `nbxmpp-4.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbxmpp
-Version: 4.3.0
+Version: 4.3.1
 Summary: XMPP Library
 Author-email: Philipp Hörist <philipp@hoerist.com>, Yann Leboulanger <yann@leboulanger.org>
 License: GPL-3.0-or-later
 Project-URL: repository, https://dev.gajim.org/gajim/python-nbxmpp
 Keywords: chat,messaging,im,xmpp
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `nbxmpp-4.3.0/README.md` & `nbxmpp-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/addresses.py` & `nbxmpp-4.3.1/nbxmpp/addresses.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/c14n.py` & `nbxmpp-4.3.1/nbxmpp/c14n.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/client.py` & `nbxmpp-4.3.1/nbxmpp/client.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/connection.py` & `nbxmpp-4.3.1/nbxmpp/connection.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/const.py` & `nbxmpp-4.3.1/nbxmpp/const.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/dispatcher.py` & `nbxmpp-4.3.1/nbxmpp/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/errors.py` & `nbxmpp-4.3.1/nbxmpp/errors.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/exceptions.py` & `nbxmpp-4.3.1/nbxmpp/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/http.py` & `nbxmpp-4.3.1/nbxmpp/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,16 @@
 
         bytes_ = data.get_data()
         if not bytes_:
             self._finish_read()
             return
 
         self._received_size += len(bytes_)
-        self._check_content_overflow()
+        if self._check_content_overflow():
+            return
 
         if self._output_stream is None:
             self._response_body_data += bytes_
 
         else:
             try:
                 self._output_stream.write_all(bytes_, self._cancellable)
@@ -443,17 +444,19 @@
 
         if not self._message.get_method() == 'GET':
             return
 
         self.emit('response-progress',
                   self._received_size / self._response_content_length)
 
-    def _check_content_overflow(self) -> None:
+    def _check_content_overflow(self) -> bool:
         if self._received_size > self._response_content_length:
             self._finish_read(HTTPRequestError.CONTENT_OVERFLOW)
+            return True
+        return False
 
     def _on_restarted(self, _message: Soup.Message) -> None:
         self._log.info('Restarted')
         self._body_received = False
         self._response_content_type = ''
         self._response_content_length = 0
         self._received_size = 0
```

### Comparing `nbxmpp-4.3.0/nbxmpp/idlequeue.py` & `nbxmpp-4.3.1/nbxmpp/idlequeue.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/activity.py` & `nbxmpp-4.3.1/nbxmpp/modules/activity.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/adhoc.py` & `nbxmpp-4.3.1/nbxmpp/modules/adhoc.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/annotations.py` & `nbxmpp-4.3.1/nbxmpp/modules/annotations.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/attention.py` & `nbxmpp-4.3.1/nbxmpp/modules/attention.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/base.py` & `nbxmpp-4.3.1/nbxmpp/modules/base.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/bits_of_binary.py` & `nbxmpp-4.3.1/nbxmpp/modules/bits_of_binary.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/blocking.py` & `nbxmpp-4.3.1/nbxmpp/modules/blocking.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/bookmarks/native_bookmarks.py` & `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/native_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/bookmarks/pep_bookmarks.py` & `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/pep_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/bookmarks/private_bookmarks.py` & `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/private_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/bookmarks/util.py` & `nbxmpp-4.3.1/nbxmpp/modules/bookmarks/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/captcha.py` & `nbxmpp-4.3.1/nbxmpp/modules/captcha.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/chat_markers.py` & `nbxmpp-4.3.1/nbxmpp/modules/chat_markers.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/chatstates.py` & `nbxmpp-4.3.1/nbxmpp/modules/chatstates.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/correction.py` & `nbxmpp-4.3.1/nbxmpp/modules/correction.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/dataforms.py` & `nbxmpp-4.3.1/nbxmpp/modules/dataforms.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/date_and_time.py` & `nbxmpp-4.3.1/nbxmpp/modules/date_and_time.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/delay.py` & `nbxmpp-4.3.1/nbxmpp/modules/delay.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/delimiter.py` & `nbxmpp-4.3.1/nbxmpp/modules/delimiter.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/discovery.py` & `nbxmpp-4.3.1/nbxmpp/modules/discovery.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/eme.py` & `nbxmpp-4.3.1/nbxmpp/modules/eme.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/entity_caps.py` & `nbxmpp-4.3.1/nbxmpp/modules/entity_caps.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/entity_time.py` & `nbxmpp-4.3.1/nbxmpp/modules/entity_time.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/http_auth.py` & `nbxmpp-4.3.1/nbxmpp/modules/http_auth.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/http_upload.py` & `nbxmpp-4.3.1/nbxmpp/modules/http_upload.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/ibb.py` & `nbxmpp-4.3.1/nbxmpp/modules/ibb.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/idle.py` & `nbxmpp-4.3.1/nbxmpp/modules/idle.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/iq.py` & `nbxmpp-4.3.1/nbxmpp/modules/iq.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/last_activity.py` & `nbxmpp-4.3.1/nbxmpp/modules/last_activity.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/location.py` & `nbxmpp-4.3.1/nbxmpp/modules/location.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/mam.py` & `nbxmpp-4.3.1/nbxmpp/modules/mam.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/message.py` & `nbxmpp-4.3.1/nbxmpp/modules/message.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/misc.py` & `nbxmpp-4.3.1/nbxmpp/modules/misc.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/mood.py` & `nbxmpp-4.3.1/nbxmpp/modules/mood.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/muc/moderation.py` & `nbxmpp-4.3.1/nbxmpp/modules/muc/moderation.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/muc/muc.py` & `nbxmpp-4.3.1/nbxmpp/modules/muc/muc.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/muc/util.py` & `nbxmpp-4.3.1/nbxmpp/modules/muc/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/muclumbus.py` & `nbxmpp-4.3.1/nbxmpp/modules/muclumbus.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/nickname.py` & `nbxmpp-4.3.1/nbxmpp/modules/nickname.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/omemo.py` & `nbxmpp-4.3.1/nbxmpp/modules/omemo.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/oob.py` & `nbxmpp-4.3.1/nbxmpp/modules/oob.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/openpgp.py` & `nbxmpp-4.3.1/nbxmpp/modules/openpgp.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/pgplegacy.py` & `nbxmpp-4.3.1/nbxmpp/modules/pgplegacy.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/ping.py` & `nbxmpp-4.3.1/nbxmpp/modules/ping.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/presence.py` & `nbxmpp-4.3.1/nbxmpp/modules/presence.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/pubsub.py` & `nbxmpp-4.3.1/nbxmpp/modules/pubsub.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/reactions.py` & `nbxmpp-4.3.1/nbxmpp/modules/reactions.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/receipts.py` & `nbxmpp-4.3.1/nbxmpp/modules/receipts.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/register/register.py` & `nbxmpp-4.3.1/nbxmpp/modules/register/register.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/register/util.py` & `nbxmpp-4.3.1/nbxmpp/modules/register/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/replies.py` & `nbxmpp-4.3.1/nbxmpp/modules/replies.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/roster.py` & `nbxmpp-4.3.1/nbxmpp/modules/roster.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/rsm.py` & `nbxmpp-4.3.1/nbxmpp/modules/rsm.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/security_labels.py` & `nbxmpp-4.3.1/nbxmpp/modules/security_labels.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/software_version.py` & `nbxmpp-4.3.1/nbxmpp/modules/software_version.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/tune.py` & `nbxmpp-4.3.1/nbxmpp/modules/tune.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/user_avatar.py` & `nbxmpp-4.3.1/nbxmpp/modules/user_avatar.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/util.py` & `nbxmpp-4.3.1/nbxmpp/modules/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/vcard4.py` & `nbxmpp-4.3.1/nbxmpp/modules/vcard4.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/vcard_avatar.py` & `nbxmpp-4.3.1/nbxmpp/modules/vcard_avatar.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/modules/vcard_temp.py` & `nbxmpp-4.3.1/nbxmpp/modules/vcard_temp.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/namespaces.py` & `nbxmpp-4.3.1/nbxmpp/namespaces.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/old_dispatcher.py` & `nbxmpp-4.3.1/nbxmpp/old_dispatcher.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/plugin.py` & `nbxmpp-4.3.1/nbxmpp/plugin.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/protocol.py` & `nbxmpp-4.3.1/nbxmpp/protocol.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/sasl.py` & `nbxmpp-4.3.1/nbxmpp/sasl.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/simplexml.py` & `nbxmpp-4.3.1/nbxmpp/simplexml.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/smacks.py` & `nbxmpp-4.3.1/nbxmpp/smacks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/stringprep.py` & `nbxmpp-4.3.1/nbxmpp/stringprep.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/structs.py` & `nbxmpp-4.3.1/nbxmpp/structs.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/task.py` & `nbxmpp-4.3.1/nbxmpp/task.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/tcp.py` & `nbxmpp-4.3.1/nbxmpp/tcp.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/third_party/hsluv.py` & `nbxmpp-4.3.1/nbxmpp/third_party/hsluv.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/util.py` & `nbxmpp-4.3.1/nbxmpp/util.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp/websocket.py` & `nbxmpp-4.3.1/nbxmpp/websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     def connect(self):
         self._log.info('Try to connect to %s', self._address.uri)
 
         self.state = TCPState.CONNECTING
 
         message = Soup.Message.new('GET', self._address.uri)
         message.connect('accept-certificate', self._check_certificate)
+        message.connect('notify::tls-peer-certificate',
+                        self._on_certificate_set)
         message.set_flags(Soup.MessageFlags.NO_REDIRECT)
         self._session.websocket_connect_async(message,
                                               None,
                                               ['xmpp'],
                                               GLib.PRIORITY_DEFAULT,
                                               self._cancellable,
                                               self._on_connect,
@@ -101,14 +103,23 @@
         if self._accept_certificate():
             return True
 
         self.notify('bad-certificate')
         self._cancellable.cancel()
         return False
 
+    def _on_certificate_set(self, message, _param):
+        if self._peer_certificate is not None:
+            return
+
+        # If the cert has errors _check_certificate() will set the cert.
+        self._peer_certificate = message.props.tls_peer_certificate
+        self._peer_certificate_errors = convert_tls_error_flags(
+            message.props.tls_peer_certificate_errors)
+
     def _on_websocket_message(self, _websocket, _type, message):
         data = message.get_data().decode()
         self._log_stanza(data)
 
         if self._input_closed:
             self._log.warning('Received data after stream closed')
             return
```

### Comparing `nbxmpp-4.3.0/nbxmpp/xmppiri.py` & `nbxmpp-4.3.1/nbxmpp/xmppiri.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/nbxmpp.egg-info/PKG-INFO` & `nbxmpp-4.3.1/nbxmpp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbxmpp
-Version: 4.3.0
+Version: 4.3.1
 Summary: XMPP Library
 Author-email: Philipp Hörist <philipp@hoerist.com>, Yann Leboulanger <yann@leboulanger.org>
 License: GPL-3.0-or-later
 Project-URL: repository, https://dev.gajim.org/gajim/python-nbxmpp
 Keywords: chat,messaging,im,xmpp
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `nbxmpp-4.3.0/nbxmpp.egg-info/SOURCES.txt` & `nbxmpp-4.3.1/nbxmpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/pyproject.toml` & `nbxmpp-4.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/lib/__init__.py` & `nbxmpp-4.3.1/test/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/lib/xmpp_mocks.py` & `nbxmpp-4.3.1/test/lib/xmpp_mocks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_activity.py` & `nbxmpp-4.3.1/test/unit/test_activity.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_avatar.py` & `nbxmpp-4.3.1/test/unit/test_avatar.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_bookmarks.py` & `nbxmpp-4.3.1/test/unit/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_datetime_parsing.py` & `nbxmpp-4.3.1/test/unit/test_datetime_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_delay_parsing.py` & `nbxmpp-4.3.1/test/unit/test_delay_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_entity_caps.py` & `nbxmpp-4.3.1/test/unit/test_entity_caps.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_error_parsing.py` & `nbxmpp-4.3.1/test/unit/test_error_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_http.py` & `nbxmpp-4.3.1/test/unit/test_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 
 from gi.repository import GLib
 from gi.repository import Soup
 
 from nbxmpp.const import HTTPRequestError
 from nbxmpp.http import HTTPSession
+from test.lib.util import raise_all_exceptions
 
 
 SMALL_FILE_URL = 'https://gajim.org/downloads/ci/unittest_small_file'  # 200 KB
 BIG_FILE_URL = 'https://gajim.org/downloads/ci/unittest_big_file'      # 7   MB
 LARGE_FILE_URL = 'https://gajim.org/downloads/ci/unittest_large_file'  # 80  MB
 NO_FILE_URL = 'https://gajim.org/downloads/ci/no-file'
 
@@ -232,10 +233,34 @@
 
         self.assertTrue(request3.is_finished())
         self.assertTrue(request3.is_complete())
 
         self.assertTrue(request4.is_finished())
         self.assertTrue(request4.is_complete())
 
+    @raise_all_exceptions
+    def test_content_overflow(self):
+
+        mainloop = GLib.MainLoop()
+
+        session = HTTPSession()
+        request = session.create_request()
+
+        def _on_starting(req) -> None:
+            req._received_size = 100000000000
+
+        callback_mock = Mock()
+        request.connect('starting-response-body', _on_starting)
+        request.connect('finished', callback_mock.finished)
+        request.connect('destroy', lambda *args: mainloop.quit())
+        request.send('GET', SMALL_FILE_URL, timeout=10)
+
+        mainloop.run()
+
+        self.assertTrue(request.is_finished())
+        self.assertFalse(request.is_complete())
+        self.assertEqual(request.get_error(), HTTPRequestError.CONTENT_OVERFLOW)
+
+        callback_mock.finished.assert_called()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `nbxmpp-4.3.0/test/unit/test_jid_parsing.py` & `nbxmpp-4.3.1/test/unit/test_jid_parsing.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_location.py` & `nbxmpp-4.3.1/test/unit/test_location.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_mood.py` & `nbxmpp-4.3.1/test/unit/test_mood.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_muclumbus.py` & `nbxmpp-4.3.1/test/unit/test_muclumbus.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_pubsub.py` & `nbxmpp-4.3.1/test/unit/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_reactions.py` & `nbxmpp-4.3.1/test/unit/test_reactions.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_sasl_scram.py` & `nbxmpp-4.3.1/test/unit/test_sasl_scram.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_stringprep.py` & `nbxmpp-4.3.1/test/unit/test_stringprep.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_tune.py` & `nbxmpp-4.3.1/test/unit/test_tune.py`

 * *Files identical despite different names*

### Comparing `nbxmpp-4.3.0/test/unit/test_xml_vulnerability.py` & `nbxmpp-4.3.1/test/unit/test_xml_vulnerability.py`

 * *Files identical despite different names*

