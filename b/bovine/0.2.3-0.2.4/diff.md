# Comparing `tmp/bovine-0.2.3.tar.gz` & `tmp/bovine-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.2.3.tar", max compression
+gzip compressed data, was "bovine-0.2.4.tar", max compression
```

## Comparing `bovine-0.2.3.tar` & `bovine-0.2.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0     1363 2023-05-27 18:25:16.679233 bovine-0.2.3/README.md
--rw-r--r--   0        0        0     9485 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 18:25:16.807235 bovine-0.2.3/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      173 2023-05-27 18:26:22.763913 bovine-0.2.3/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3741 2023-05-27 18:26:22.763913 bovine-0.2.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     2475 2023-05-27 18:26:23.275918 bovine-0.2.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0      922 2023-05-27 18:26:23.399919 bovine-0.2.3/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
--rw-r--r--   0        0        0     3638 2023-05-27 18:26:23.731922 bovine-0.2.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1212 2023-05-27 18:26:23.751923 bovine-0.2.3/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3505 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2542 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      434 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      498 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/test_collection_helper.py
--rw-r--r--   0        0        0     4957 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4645 2023-05-27 18:26:23.391919 bovine-0.2.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4269 2023-05-27 18:26:23.395919 bovine-0.2.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4028 2023-05-27 18:26:23.395919 bovine-0.2.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4584 2023-05-27 18:26:23.759923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3327 2023-05-27 18:26:23.767923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3113 2023-05-27 18:26:23.775923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1951 2023-05-27 18:26:23.779923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1386 2023-05-27 18:26:23.779923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4203 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4178 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2195 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1442 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1257 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1034 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      817 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2836 2023-05-27 18:26:23.395919 bovine-0.2.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      972 2023-05-27 18:26:23.399919 bovine-0.2.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
--rw-r--r--   0        0        0     4763 2023-05-27 18:26:23.791923 bovine-0.2.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      865 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     3968 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/__init__.py
--rw-r--r--   0        0        0     4002 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-05-27 18:26:23.059916 bovine-0.2.3/bovine/clients/__pycache__/bearer.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1719 2023-05-27 18:26:23.107916 bovine-0.2.3/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1084 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2534 2023-05-27 18:26:23.111916 bovine-0.2.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
--rw-r--r--   0        0        0     1237 2023-05-27 18:26:23.059916 bovine-0.2.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     1529 2023-05-27 18:26:23.275918 bovine-0.2.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     2479 2023-05-27 18:26:23.275918 bovine-0.2.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
--rw-r--r--   0        0        0     1507 2023-05-27 18:26:23.795923 bovine-0.2.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2844 2023-05-27 18:26:23.799923 bovine-0.2.3/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1217 2023-05-27 18:26:23.803923 bovine-0.2.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2102 2023-05-27 18:26:23.807923 bovine-0.2.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      814 2023-05-27 18:26:23.807923 bovine-0.2.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1794 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/bearer.py
--rw-r--r--   0        0        0       91 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/consts.py
--rw-r--r--   0        0        0     1520 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/event_source.py
--rw-r--r--   0        0        0      868 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3001 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/moo_auth.py
--rw-r--r--   0        0        0      948 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     1150 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     3278 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/signed_http_methods.py
--rw-r--r--   0        0        0      651 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0     1505 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1153 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      522 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     4141 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3749 2023-05-27 18:26:23.111916 bovine-0.2.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2863 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2909 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2257 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2363 2023-05-27 18:26:23.747923 bovine-0.2.3/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5821 2023-05-27 18:26:23.815923 bovine-0.2.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2742 2023-05-27 18:26:23.819923 bovine-0.2.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     7454 2023-05-27 18:26:23.831924 bovine-0.2.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2674 2023-05-27 18:26:23.839924 bovine-0.2.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2664 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test.py
--rw-r--r--   0        0        0     4995 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/ed25519_key.py
--rw-r--r--   0        0        0     3342 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/jsonld.py
--rw-r--r--   0        0        0      864 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/msg.py
--rw-r--r--   0        0        0     3256 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/repl.py
--rw-r--r--   0        0        0      178 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/test_bovine_client.py
--rw-r--r--   0        0        0     5250 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/test_jsonld.py
--rw-r--r--   0        0        0      282 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/types.py
--rw-r--r--   0        0        0      856 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/__init__.py
--rw-r--r--   0        0        0     1120 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      877 2023-05-27 18:26:23.059916 bovine-0.2.3/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0     3240 2023-05-27 18:26:23.715922 bovine-0.2.3/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc
--rw-r--r--   0        0        0     3465 2023-05-27 18:26:23.847924 bovine-0.2.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1662 2023-05-27 18:26:23.851924 bovine-0.2.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1625 2023-05-27 18:26:23.851924 bovine-0.2.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      519 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/date.py
--rw-r--r--   0        0        0     1432 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0     1934 2023-05-27 18:26:23.855924 bovine-0.2.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1967 2023-05-27 18:26:23.859924 bovine-0.2.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      659 2023-05-27 18:26:23.855924 bovine-0.2.3/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0      599 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      261 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0     4736 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/pyld_requests.py
--rw-r--r--   0        0        0      761 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      368 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1405 2023-05-27 18:25:16.683233 bovine-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bovine-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1363 2023-05-27 18:46:13.768355 bovine-0.2.4/README.md
+-rw-r--r--   0        0        0     9485 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 18:46:13.932356 bovine-0.2.4/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-27 18:47:14.456986 bovine-0.2.4/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3741 2023-05-27 18:47:14.456986 bovine-0.2.4/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2173 2023-05-27 18:47:14.964991 bovine-0.2.4/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      922 2023-05-27 18:47:15.104992 bovine-0.2.4/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-05-27 18:47:15.444996 bovine-0.2.4/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1212 2023-05-27 18:47:15.464996 bovine-0.2.4/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3505 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2255 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      434 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0      498 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitypub/test_collection_helper.py
+-rw-r--r--   0        0        0     4957 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4645 2023-05-27 18:47:14.964991 bovine-0.2.4/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4269 2023-05-27 18:47:14.968991 bovine-0.2.4/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4028 2023-05-27 18:47:14.968991 bovine-0.2.4/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4584 2023-05-27 18:47:15.476996 bovine-0.2.4/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3327 2023-05-27 18:47:15.484996 bovine-0.2.4/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3113 2023-05-27 18:47:15.488997 bovine-0.2.4/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1951 2023-05-27 18:47:15.492997 bovine-0.2.4/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1386 2023-05-27 18:47:15.496996 bovine-0.2.4/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4203 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4178 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1257 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-05-27 18:47:14.968991 bovine-0.2.4/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      972 2023-05-27 18:47:14.972991 bovine-0.2.4/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-05-27 18:47:15.504997 bovine-0.2.4/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      865 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     3968 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     4002 2023-05-27 18:47:14.748989 bovine-0.2.4/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-05-27 18:47:14.752989 bovine-0.2.4/bovine/clients/__pycache__/bearer.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-05-27 18:47:14.748989 bovine-0.2.4/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1719 2023-05-27 18:47:14.796989 bovine-0.2.4/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1084 2023-05-27 18:47:14.748989 bovine-0.2.4/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2534 2023-05-27 18:47:14.800989 bovine-0.2.4/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-05-27 18:47:14.752989 bovine-0.2.4/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     1529 2023-05-27 18:47:14.964991 bovine-0.2.4/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     2479 2023-05-27 18:47:14.964991 bovine-0.2.4/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
+-rw-r--r--   0        0        0     1507 2023-05-27 18:47:15.512997 bovine-0.2.4/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2844 2023-05-27 18:47:15.516997 bovine-0.2.4/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1217 2023-05-27 18:47:15.516997 bovine-0.2.4/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2102 2023-05-27 18:47:15.520997 bovine-0.2.4/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      814 2023-05-27 18:47:15.524997 bovine-0.2.4/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1794 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      868 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-05-27 18:46:13.768355 bovine-0.2.4/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      651 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1505 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3749 2023-05-27 18:47:14.800989 bovine-0.2.4/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-05-27 18:47:14.960991 bovine-0.2.4/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-05-27 18:47:14.960991 bovine-0.2.4/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-05-27 18:47:14.960991 bovine-0.2.4/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-05-27 18:47:14.960991 bovine-0.2.4/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-05-27 18:47:15.464996 bovine-0.2.4/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5821 2023-05-27 18:47:15.532997 bovine-0.2.4/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2742 2023-05-27 18:47:15.536997 bovine-0.2.4/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     7454 2023-05-27 18:47:15.544997 bovine-0.2.4/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2674 2023-05-27 18:47:15.552997 bovine-0.2.4/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2664 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/ed25519_key.py
+-rw-r--r--   0        0        0     3342 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/jsonld.py
+-rw-r--r--   0        0        0      864 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/msg.py
+-rw-r--r--   0        0        0     3256 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/repl.py
+-rw-r--r--   0        0        0      178 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0     5250 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/test_jsonld.py
+-rw-r--r--   0        0        0      282 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/types.py
+-rw-r--r--   0        0        0      856 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2023-05-27 18:47:14.748989 bovine-0.2.4/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-05-27 18:47:14.752989 bovine-0.2.4/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3240 2023-05-27 18:47:15.432996 bovine-0.2.4/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-05-27 18:47:15.560997 bovine-0.2.4/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1662 2023-05-27 18:47:15.564997 bovine-0.2.4/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1625 2023-05-27 18:47:15.568997 bovine-0.2.4/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      519 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/date.py
+-rw-r--r--   0        0        0     1432 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0     1934 2023-05-27 18:47:15.568997 bovine-0.2.4/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1967 2023-05-27 18:47:15.572997 bovine-0.2.4/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      659 2023-05-27 18:47:15.572997 bovine-0.2.4/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      599 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0     4736 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/pyld_requests.py
+-rw-r--r--   0        0        0      761 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      368 2023-05-27 18:46:13.772355 bovine-0.2.4/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1405 2023-05-27 18:46:13.780355 bovine-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bovine-0.2.4/PKG-INFO
```

### Comparing `bovine-0.2.3/README.md` & `bovine-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/__init__.py` & `bovine-0.2.4/bovine/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc` & `bovine-0.2.4/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 3505 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 b10d 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 b10d 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `bovine-0.2.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc` & `bovine-0.2.4/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2542 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,155 +1,136 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 ee09 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 cf08 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
-00000050: 6406 8400 5a05 6407 6408 8400 5a06 4700  d...Z.d.d...Z.G.
-00000060: 6409 640a 8400 640a 8302 5a07 6401 5300  d.d...d...Z.d.S.
-00000070: 290b e900 0000 004e 2901 da0e 7072 696e  )......N)...prin
-00000080: 745f 6163 7469 7669 7479 e901 0000 00a9  t_activity......
-00000090: 01da 1243 6f6c 6c65 6374 696f 6e49 7465  ...CollectionIte
-000000a0: 7261 746f 7263 0200 0000 0000 0000 0000  ratorc..........
-000000b0: 0000 0300 0000 0500 0000 c300 0000 7384  ..............s.
-000000c0: 0000 0081 0167 007d 0274 007c 0174 0183  .....g.}.t.|.t..
-000000d0: 0272 107c 00a0 027c 01a1 0149 0064 0048  .r.|...|...I.d.H
-000000e0: 007d 0164 017c 0176 0072 207c 0164 0119  .}.d.|.v.r |.d..
-000000f0: 007d 0274 007c 0274 0183 0272 207c 0267  .}.t.|.t...r |.g
-00000100: 017d 0264 027c 0176 0072 307c 0274 037c  .}.d.|.v.r0|.t.|
-00000110: 007c 0164 0219 0083 0249 0064 0048 0017  .|.d.....I.d.H..
-00000120: 0053 0064 037c 0176 0072 407c 0274 037c  .S.d.|.v.r@|.t.|
-00000130: 007c 0164 0319 0083 0249 0064 0048 0017  .|.d.....I.d.H..
-00000140: 0053 007c 0253 0029 044e da05 6974 656d  .S.|.S.).N..item
-00000150: 73da 0566 6972 7374 da04 6e65 7874 2904  s..first..next).
-00000160: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
-00000170: 72da 0d70 726f 7879 5f65 6c65 6d65 6e74  r..proxy_element
-00000180: da17 616c 6c5f 636f 6c6c 6563 7469 6f6e  ..all_collection
-00000190: 5f65 6c65 6d65 6e74 7329 03da 0663 6c69  _elements)...cli
-000001a0: 656e 74da 0a63 6f6c 6c65 6374 696f 6eda  ent..collection.
-000001b0: 0672 6573 756c 74a9 0072 1000 0000 fa59  .result..r.....Y
-000001c0: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-000001d0: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
-000001e0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-000001f0: 652f 626f 7669 6e65 2f61 6374 6976 6974  e/bovine/activit
-00000200: 7970 7562 2f63 6f6c 6c65 6374 696f 6e5f  ypub/collection_
-00000210: 6865 6c70 6572 2e70 7972 0c00 0000 0800  helper.pyr......
-00000220: 0000 731a 0000 0002 8004 010a 0110 0108  ..s.............
-00000230: 0208 010a 0106 0108 0218 0108 0218 0104  ................
-00000240: 0272 0c00 0000 6301 0000 0000 0000 0000  .r....c.........
-00000250: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00000260: 4600 0000 6401 7c00 7600 7208 7c00 6401  F...d.|.v.r.|.d.
-00000270: 1900 7d00 6402 4400 5d16 7d01 7c01 7c00  ..}.d.D.].}.|.|.
-00000280: 7600 7220 7c00 7c01 1900 7220 7400 6a01  v.r |.|...r t.j.
-00000290: 7c00 7c01 1900 6700 6403 6404 8d03 0200  |.|...g.d.d.....
-000002a0: 0100 5300 710a 6405 5300 2906 4eda 066f  ..S.q.d.S.).N..o
-000002b0: 626a 6563 7429 04da 046e 616d 65da 0773  bject)...name..s
-000002c0: 756d 6d61 7279 da07 636f 6e74 656e 74da  ummary..content.
-000002d0: 0269 6454 2902 da04 7461 6773 da05 7374  .idT)...tags..st
-000002e0: 7269 707a 102d 2d2d 2075 6e6b 6e6f 776e  ripz.--- unknown
-000002f0: 2020 2d2d 2d29 02da 0662 6c65 6163 68da    ---)...bleach.
-00000300: 0563 6c65 616e 2902 da03 6f62 6ada 036b  .clean)...obj..k
-00000310: 6579 7210 0000 0072 1000 0000 7211 0000  eyr....r....r...
-00000320: 00da 1773 686f 7274 5f76 6572 7369 6f6e  ...short_version
-00000330: 5f6f 665f 6f62 6a65 6374 1b00 0000 730e  _of_object....s.
-00000340: 0000 0008 0108 0108 0210 0118 0102 8004  ................
-00000350: 0272 1d00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000360: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00000370: 3800 0000 6500 5a01 6400 5a02 6401 6402  8...e.Z.d.Z.d.d.
-00000380: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-00000390: 8400 5a05 640e 6408 6409 8401 5a06 640f  ..Z.d.d.d...Z.d.
-000003a0: 640b 640c 8401 5a07 640d 5300 2910 da10  d.d...Z.d.S.)...
-000003b0: 436f 6c6c 6563 7469 6f6e 4865 6c70 6572  CollectionHelper
-000003c0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000003d0: 0002 0000 0043 0000 0073 2e00 0000 7c01  .....C...s....|.
-000003e0: 7c00 5f00 7c02 7c00 5f01 6400 7c00 5f02  |._.|.|._.d.|._.
-000003f0: 6400 7c00 5f03 6400 7c00 5f04 6400 7c00  d.|._.d.|._.d.|.
-00000400: 5f05 6900 7c00 5f06 6400 5300 a901 4e29  _.i.|._.d.S...N)
-00000410: 07da 0d63 6f6c 6c65 6374 696f 6e5f 6964  ...collection_id
-00000420: da05 6163 746f 72da 1162 6173 6963 5f69  ..actor..basic_i
-00000430: 6e66 6f72 6d61 7469 6f6e 7206 0000 00da  nformationr.....
-00000440: 0a6e 6578 745f 6974 656d 73da 0a69 7465  .next_items..ite
-00000450: 6d5f 696e 6465 78da 0d65 6c65 6d65 6e74  m_index..element
-00000460: 5f63 6163 6865 2903 da04 7365 6c66 7220  _cache)...selfr 
-00000470: 0000 0072 2100 0000 7210 0000 0072 1000  ...r!...r....r..
-00000480: 0000 7211 0000 00da 085f 5f69 6e69 745f  ..r......__init_
-00000490: 5f27 0000 0073 0e00 0000 0601 0601 0602  _'...s..........
-000004a0: 0601 0601 0601 0a02 7a19 436f 6c6c 6563  ........z.Collec
-000004b0: 7469 6f6e 4865 6c70 6572 2e5f 5f69 6e69  tionHelper.__ini
-000004c0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-000004d0: 0200 0000 0400 0000 c300 0000 7366 0000  ............sf..
-000004e0: 0081 017c 006a 0064 0075 0072 117c 006a  ...|.j.d.u.r.|.j
-000004f0: 01a0 027c 006a 03a1 0149 0064 0048 007c  ...|.j...I.d.H.|
-00000500: 005f 0064 017c 006a 0076 0172 1864 0053  ._.d.|.j.v.r.d.S
-00000510: 007c 006a 01a0 027c 006a 0064 0119 00a1  .|.j...|.j.d....
-00000520: 0149 0064 0048 007d 017c 0164 0219 007c  .I.d.H.}.|.d...|
-00000530: 005f 047c 0164 0319 007c 005f 0564 047c  ._.|.d...|._.d.|
-00000540: 005f 0664 0053 0029 054e 7207 0000 00da  ._.d.S.).Nr.....
-00000550: 0c6f 7264 6572 6564 4974 656d 7372 0800  .orderedItemsr..
-00000560: 0000 7201 0000 0029 0772 2200 0000 7221  ..r....).r"...r!
-00000570: 0000 00da 0367 6574 7220 0000 0072 0600  .....getr ...r..
-00000580: 0000 7223 0000 0072 2400 0000 2902 7226  ..r#...r$...).r&
-00000590: 0000 00da 0872 6573 706f 6e73 6572 1000  .....responser..
-000005a0: 0000 7210 0000 0072 1100 0000 da07 7265  ..r....r......re
-000005b0: 6672 6573 6832 0000 0073 1200 0000 0280  fresh2...s......
-000005c0: 0a01 1601 0a02 0401 1802 0a02 0a01 0a01  ................
-000005d0: 7a18 436f 6c6c 6563 7469 6f6e 4865 6c70  z.CollectionHelp
-000005e0: 6572 2e72 6566 7265 7368 6302 0000 0000  er.refreshc.....
-000005f0: 0000 0000 0000 0003 0000 0003 0000 00c3  ................
-00000600: 0000 0073 4400 0000 8101 7400 7c01 7401  ...sD.....t.|.t.
-00000610: 8302 7308 7c01 5300 7c01 7c00 6a02 7600  ..s.|.S.|.|.j.v.
-00000620: 7212 7c00 6a02 7c01 1900 5300 7c00 6a03  r.|.j.|...S.|.j.
-00000630: a004 7c01 a101 4900 6400 4800 7d02 7c02  ..|...I.d.H.}.|.
-00000640: 7c00 6a02 7c01 3c00 7c02 5300 721f 0000  |.j.|.<.|.S.r...
-00000650: 0029 0572 0900 0000 720a 0000 0072 2500  .).r....r....r%.
-00000660: 0000 7221 0000 0072 0b00 0000 2903 7226  ..r!...r....).r&
-00000670: 0000 00da 0765 6c65 6d65 6e74 720f 0000  .....elementr...
-00000680: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000690: da0b 6765 745f 656c 656d 656e 743f 0000  ..get_element?..
-000006a0: 0073 1000 0000 0280 0a01 0401 0a02 0a01  .s..............
-000006b0: 1202 0a02 0402 7a1c 436f 6c6c 6563 7469  ......z.Collecti
-000006c0: 6f6e 4865 6c70 6572 2e67 6574 5f65 6c65  onHelper.get_ele
-000006d0: 6d65 6e74 4663 0200 0000 0000 0000 0000  mentFc..........
-000006e0: 0000 0400 0000 0400 0000 c300 0000 737c  ..............s|
-000006f0: 0000 0081 017c 006a 0074 017c 006a 0283  .....|.j.t.|.j..
-00000700: 016b 0572 217c 006a 03a0 047c 006a 05a1  .k.r!|.j...|.j..
-00000710: 0149 0064 0048 007d 027c 0004 006a 027c  .I.d.H.}.|...j.|
-00000720: 0264 0119 0037 0002 005f 027c 0264 0219  .d...7..._.|.d..
-00000730: 007c 005f 057c 006a 027c 006a 0019 007d  .|._.|.j.|.j...}
-00000740: 037c 0004 006a 0064 0337 0002 005f 007c  .|...j.d.7..._.|
-00000750: 00a0 067c 03a1 0149 0064 0048 007d 037c  ...|...I.d.H.}.|
-00000760: 0172 3c74 077c 0383 0101 007c 0353 0029  .r<t.|.....|.S.)
-00000770: 044e 7228 0000 0072 0800 0000 7203 0000  .Nr(...r....r...
-00000780: 0029 0872 2400 0000 da03 6c65 6e72 0600  .).r$.....lenr..
-00000790: 0000 7221 0000 0072 2900 0000 7223 0000  ..r!...r)...r#..
-000007a0: 0072 2d00 0000 7202 0000 0029 0472 2600  .r-...r....).r&.
-000007b0: 0000 5a08 646f 5f70 7269 6e74 722a 0000  ..Z.do_printr*..
-000007c0: 0072 0f00 0000 7210 0000 0072 1000 0000  .r....r....r....
-000007d0: 7211 0000 00da 096e 6578 745f 6974 656d  r......next_item
-000007e0: 4c00 0000 7316 0000 0002 8010 0114 0112  L...s...........
-000007f0: 010a 010c 020e 0110 0204 0208 0104 027a  ...............z
-00000800: 1a43 6f6c 6c65 6374 696f 6e48 656c 7065  .CollectionHelpe
-00000810: 722e 6e65 7874 5f69 7465 6de9 0a00 0000  r.next_item.....
-00000820: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000830: 0003 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
-00000840: 7c00 7c01 8302 5300 721f 0000 0072 0400  |.|...S.r....r..
-00000850: 0000 2902 7226 0000 005a 0a6d 6178 5f6e  ..).r&...Z.max_n
-00000860: 756d 6265 7272 1000 0000 7210 0000 0072  umberr....r....r
-00000870: 1100 0000 da07 6974 6572 6174 655c 0000  ......iterate\..
-00000880: 0073 0200 0000 0a01 7a18 436f 6c6c 6563  .s......z.Collec
-00000890: 7469 6f6e 4865 6c70 6572 2e69 7465 7261  tionHelper.itera
-000008a0: 7465 4e29 0146 2901 7230 0000 0029 08da  teN).F).r0...)..
-000008b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000008c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000008d0: 655f 5f72 2700 0000 722b 0000 0072 2d00  e__r'...r+...r-.
-000008e0: 0000 722f 0000 0072 3100 0000 7210 0000  ..r/...r1...r...
-000008f0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000900: 721e 0000 0026 0000 0073 0c00 0000 0800  r....&...s......
-00000910: 0801 080b 080d 0a0d 0e10 721e 0000 0029  ..........r....)
-00000920: 0872 1900 0000 5a22 626f 7669 6e65 2e61  .r....Z"bovine.a
-00000930: 6374 6976 6974 7973 7472 6561 6d73 2e75  ctivitystreams.u
-00000940: 7469 6c73 2e70 7269 6e74 7202 0000 005a  tils.printr....Z
-00000950: 1363 6f6c 6c65 6374 696f 6e5f 6974 6572  .collection_iter
-00000960: 6174 6f72 7205 0000 0072 0c00 0000 721d  atorr....r....r.
-00000970: 0000 0072 1e00 0000 7210 0000 0072 1000  ...r....r....r..
-00000980: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
-00000990: 6f64 756c 653e 0100 0000 730c 0000 0008  odule>....s.....
-000009a0: 000c 020c 0208 0308 1312 0b              ...........
+00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
+00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 0100 6404 6405 8400 5a04 4700  m.Z...d.d...Z.G.
+00000050: 6406 6407 8400 6407 8302 5a05 6408 5300  d.d...d...Z.d.S.
+00000060: 2909 e900 0000 0029 01da 0e70 7269 6e74  )......)...print
+00000070: 5f61 6374 6976 6974 79e9 0100 0000 a901  _activity.......
+00000080: da12 436f 6c6c 6563 7469 6f6e 4974 6572  ..CollectionIter
+00000090: 6174 6f72 6302 0000 0000 0000 0000 0000  atorc...........
+000000a0: 0003 0000 0005 0000 00c3 0000 0073 8400  .............s..
+000000b0: 0000 8101 6700 7d02 7400 7c01 7401 8302  ....g.}.t.|.t...
+000000c0: 7210 7c00 a002 7c01 a101 4900 6400 4800  r.|...|...I.d.H.
+000000d0: 7d01 6401 7c01 7600 7220 7c01 6401 1900  }.d.|.v.r |.d...
+000000e0: 7d02 7400 7c02 7401 8302 7220 7c02 6701  }.t.|.t...r |.g.
+000000f0: 7d02 6402 7c01 7600 7230 7c02 7403 7c00  }.d.|.v.r0|.t.|.
+00000100: 7c01 6402 1900 8302 4900 6400 4800 1700  |.d.....I.d.H...
+00000110: 5300 6403 7c01 7600 7240 7c02 7403 7c00  S.d.|.v.r@|.t.|.
+00000120: 7c01 6403 1900 8302 4900 6400 4800 1700  |.d.....I.d.H...
+00000130: 5300 7c02 5300 2904 4eda 0569 7465 6d73  S.|.S.).N..items
+00000140: da05 6669 7273 74da 046e 6578 7429 04da  ..first..next)..
+00000150: 0a69 7369 6e73 7461 6e63 65da 0373 7472  .isinstance..str
+00000160: da0d 7072 6f78 795f 656c 656d 656e 74da  ..proxy_element.
+00000170: 1761 6c6c 5f63 6f6c 6c65 6374 696f 6e5f  .all_collection_
+00000180: 656c 656d 656e 7473 2903 da06 636c 6965  elements)...clie
+00000190: 6e74 da0a 636f 6c6c 6563 7469 6f6e da06  nt..collection..
+000001a0: 7265 7375 6c74 a900 7210 0000 00fa 592f  result..r.....Y/
+000001b0: 776f 6f64 7065 636b 6572 2f73 7263 2f63  woodpecker/src/c
+000001c0: 6f64 6562 6572 672e 6f72 672f 626f 7669  odeberg.org/bovi
+000001d0: 6e65 2f62 6f76 696e 652f 626f 7669 6e65  ne/bovine/bovine
+000001e0: 2f62 6f76 696e 652f 6163 7469 7669 7479  /bovine/activity
+000001f0: 7075 622f 636f 6c6c 6563 7469 6f6e 5f68  pub/collection_h
+00000200: 656c 7065 722e 7079 720c 0000 0006 0000  elper.pyr.......
+00000210: 0073 1a00 0000 0280 0401 0a01 1001 0802  .s..............
+00000220: 0801 0a01 0601 0802 1801 0802 1801 0402  ................
+00000230: 720c 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000240: 0000 0000 0000 0300 0000 4000 0000 7338  ..........@...s8
+00000250: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00000260: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+00000270: 005a 0564 0e64 0864 0984 015a 0664 0f64  .Z.d.d.d...Z.d.d
+00000280: 0b64 0c84 015a 0764 0d53 0029 10da 1043  .d...Z.d.S.)...C
+00000290: 6f6c 6c65 6374 696f 6e48 656c 7065 7263  ollectionHelperc
+000002a0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+000002b0: 0200 0000 4300 0000 732e 0000 007c 017c  ....C...s....|.|
+000002c0: 005f 007c 027c 005f 0164 007c 005f 0264  ._.|.|._.d.|._.d
+000002d0: 007c 005f 0364 007c 005f 0464 007c 005f  .|._.d.|._.d.|._
+000002e0: 0569 007c 005f 0664 0053 00a9 014e 2907  .i.|._.d.S...N).
+000002f0: da0d 636f 6c6c 6563 7469 6f6e 5f69 64da  ..collection_id.
+00000300: 0561 6374 6f72 da11 6261 7369 635f 696e  .actor..basic_in
+00000310: 666f 726d 6174 696f 6e72 0600 0000 da0a  formationr......
+00000320: 6e65 7874 5f69 7465 6d73 da0a 6974 656d  next_items..item
+00000330: 5f69 6e64 6578 da0d 656c 656d 656e 745f  _index..element_
+00000340: 6361 6368 6529 03da 0473 656c 6672 1400  cache)...selfr..
+00000350: 0000 7215 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000360: 0072 1100 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+00000370: 1a00 0000 730e 0000 0006 0106 0106 0206  ....s...........
+00000380: 0106 0106 010a 027a 1943 6f6c 6c65 6374  .......z.Collect
+00000390: 696f 6e48 656c 7065 722e 5f5f 696e 6974  ionHelper.__init
+000003a0: 5f5f 6301 0000 0000 0000 0000 0000 0002  __c.............
+000003b0: 0000 0004 0000 00c3 0000 0073 6600 0000  ...........sf...
+000003c0: 8101 7c00 6a00 6400 7500 7211 7c00 6a01  ..|.j.d.u.r.|.j.
+000003d0: a002 7c00 6a03 a101 4900 6400 4800 7c00  ..|.j...I.d.H.|.
+000003e0: 5f00 6401 7c00 6a00 7601 7218 6400 5300  _.d.|.j.v.r.d.S.
+000003f0: 7c00 6a01 a002 7c00 6a00 6401 1900 a101  |.j...|.j.d.....
+00000400: 4900 6400 4800 7d01 7c01 6402 1900 7c00  I.d.H.}.|.d...|.
+00000410: 5f04 7c01 6403 1900 7c00 5f05 6404 7c00  _.|.d...|._.d.|.
+00000420: 5f06 6400 5300 2905 4e72 0700 0000 da0c  _.d.S.).Nr......
+00000430: 6f72 6465 7265 6449 7465 6d73 7208 0000  orderedItemsr...
+00000440: 0072 0100 0000 2907 7216 0000 0072 1500  .r....).r....r..
+00000450: 0000 da03 6765 7472 1400 0000 7206 0000  ....getr....r...
+00000460: 0072 1700 0000 7218 0000 0029 0272 1a00  .r....r....).r..
+00000470: 0000 da08 7265 7370 6f6e 7365 7210 0000  ....responser...
+00000480: 0072 1000 0000 7211 0000 00da 0772 6566  .r....r......ref
+00000490: 7265 7368 2500 0000 7312 0000 0002 800a  resh%...s.......
+000004a0: 0116 010a 0204 0118 020a 020a 010a 017a  ...............z
+000004b0: 1843 6f6c 6c65 6374 696f 6e48 656c 7065  .CollectionHelpe
+000004c0: 722e 7265 6672 6573 6863 0200 0000 0000  r.refreshc......
+000004d0: 0000 0000 0000 0300 0000 0300 0000 c300  ................
+000004e0: 0000 7344 0000 0081 0174 007c 0174 0183  ..sD.....t.|.t..
+000004f0: 0273 087c 0153 007c 017c 006a 0276 0072  .s.|.S.|.|.j.v.r
+00000500: 127c 006a 027c 0119 0053 007c 006a 03a0  .|.j.|...S.|.j..
+00000510: 047c 01a1 0149 0064 0048 007d 027c 027c  .|...I.d.H.}.|.|
+00000520: 006a 027c 013c 007c 0253 0072 1300 0000  .j.|.<.|.S.r....
+00000530: 2905 7209 0000 0072 0a00 0000 7219 0000  ).r....r....r...
+00000540: 0072 1500 0000 720b 0000 0029 0372 1a00  .r....r....).r..
+00000550: 0000 da07 656c 656d 656e 7472 0f00 0000  ....elementr....
+00000560: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000570: 0b67 6574 5f65 6c65 6d65 6e74 3200 0000  .get_element2...
+00000580: 7310 0000 0002 800a 0104 010a 020a 0112  s...............
+00000590: 020a 0204 027a 1c43 6f6c 6c65 6374 696f  .....z.Collectio
+000005a0: 6e48 656c 7065 722e 6765 745f 656c 656d  nHelper.get_elem
+000005b0: 656e 7446 6302 0000 0000 0000 0000 0000  entFc...........
+000005c0: 0004 0000 0004 0000 00c3 0000 0073 7c00  .............s|.
+000005d0: 0000 8101 7c00 6a00 7401 7c00 6a02 8301  ....|.j.t.|.j...
+000005e0: 6b05 7221 7c00 6a03 a004 7c00 6a05 a101  k.r!|.j...|.j...
+000005f0: 4900 6400 4800 7d02 7c00 0400 6a02 7c02  I.d.H.}.|...j.|.
+00000600: 6401 1900 3700 0200 5f02 7c02 6402 1900  d...7..._.|.d...
+00000610: 7c00 5f05 7c00 6a02 7c00 6a00 1900 7d03  |._.|.j.|.j...}.
+00000620: 7c00 0400 6a00 6403 3700 0200 5f00 7c00  |...j.d.7..._.|.
+00000630: a006 7c03 a101 4900 6400 4800 7d03 7c01  ..|...I.d.H.}.|.
+00000640: 723c 7407 7c03 8301 0100 7c03 5300 2904  r<t.|.....|.S.).
+00000650: 4e72 1c00 0000 7208 0000 0072 0300 0000  Nr....r....r....
+00000660: 2908 7218 0000 00da 036c 656e 7206 0000  ).r......lenr...
+00000670: 0072 1500 0000 721d 0000 0072 1700 0000  .r....r....r....
+00000680: 7221 0000 0072 0200 0000 2904 721a 0000  r!...r....).r...
+00000690: 005a 0864 6f5f 7072 696e 7472 1e00 0000  .Z.do_printr....
+000006a0: 720f 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+000006b0: 1100 0000 da09 6e65 7874 5f69 7465 6d3f  ......next_item?
+000006c0: 0000 0073 1600 0000 0280 1001 1401 1201  ...s............
+000006d0: 0a01 0c02 0e01 1002 0402 0801 0402 7a1a  ..............z.
+000006e0: 436f 6c6c 6563 7469 6f6e 4865 6c70 6572  CollectionHelper
+000006f0: 2e6e 6578 745f 6974 656d e90a 0000 0063  .next_item.....c
+00000700: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000710: 0300 0000 4300 0000 730a 0000 0074 007c  ....C...s....t.|
+00000720: 007c 0183 0253 0072 1300 0000 7204 0000  .|...S.r....r...
+00000730: 0029 0272 1a00 0000 5a0a 6d61 785f 6e75  .).r....Z.max_nu
+00000740: 6d62 6572 7210 0000 0072 1000 0000 7211  mberr....r....r.
+00000750: 0000 00da 0769 7465 7261 7465 4f00 0000  .....iterateO...
+00000760: 7302 0000 000a 017a 1843 6f6c 6c65 6374  s......z.Collect
+00000770: 696f 6e48 656c 7065 722e 6974 6572 6174  ionHelper.iterat
+00000780: 654e 2901 4629 0172 2400 0000 2908 da08  eN).F).r$...)...
+00000790: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000007a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000007b0: 5f5f 721b 0000 0072 1f00 0000 7221 0000  __r....r....r!..
+000007c0: 0072 2300 0000 7225 0000 0072 1000 0000  .r#...r%...r....
+000007d0: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000007e0: 1200 0000 1900 0000 730c 0000 0008 0008  ........s.......
+000007f0: 0108 0b08 0d0a 0d0e 1072 1200 0000 4e29  .........r....N)
+00000800: 065a 2262 6f76 696e 652e 6163 7469 7669  .Z"bovine.activi
+00000810: 7479 7374 7265 616d 732e 7574 696c 732e  tystreams.utils.
+00000820: 7072 696e 7472 0200 0000 5a13 636f 6c6c  printr....Z.coll
+00000830: 6563 7469 6f6e 5f69 7465 7261 746f 7272  ection_iteratorr
+00000840: 0500 0000 720c 0000 0072 1200 0000 7210  ....r....r....r.
+00000850: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+00000860: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000870: 7308 0000 000c 000c 0208 0312 13         s............
```

### Comparing `bovine-0.2.3/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc` & `bovine-0.2.4/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 b201 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 b201 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 0003 0000 0040 0000 0073 2a00 0000  .......@...s*...
 00000060: 6500 5a01 6400 5a02 6401 6503 6602 6402  e.Z.d.Z.d.e.f.d.
 00000070: 6403 8404 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.2.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 c50a 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 c50a 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6400 6401 6c0a 5a0a 6400 6403 6c0b 6d0c  d.d.l.Z.d.d.l.m.
 00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `bovine-0.2.3/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 498 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 f201 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 f201 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6403 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6506 6a0b a00c 6405  l.m.Z...e.j...d.
 00000070: a101 6406 6407 8400 8301 5a0d 6401 5300  ..d.d.....Z.d.S.
```

### Comparing `bovine-0.2.3/bovine/activitypub/authorization_wrapper.py` & `bovine-0.2.4/bovine/activitypub/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitypub/collection_helper.py` & `bovine-0.2.4/bovine/activitypub/collection_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import bleach
-
 from bovine.activitystreams.utils.print import print_activity
 
 from .collection_iterator import CollectionIterator
 
 
 async def all_collection_elements(client, collection):
     result = []
@@ -20,25 +18,14 @@
 
     if "next" in collection:
         return result + await all_collection_elements(client, collection["next"])
 
     return result
 
 
-def short_version_of_object(obj):
-    if "object" in obj:
-        obj = obj["object"]
-
-    for key in ["name", "summary", "content", "id"]:
-        if key in obj and obj[key]:
-            return bleach.clean(obj[key], tags=[], strip=True)
-
-    return "--- unknown  ---"
-
-
 class CollectionHelper:
     def __init__(self, collection_id, actor):
         self.collection_id = collection_id
         self.actor = actor
 
         self.basic_information = None
         self.items = None
```

### Comparing `bovine-0.2.3/bovine/activitypub/test_actor.py` & `bovine-0.2.4/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/__init__.py` & `bovine-0.2.4/bovine/activitystreams/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 4957 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 5d13 0000  o........Krd]...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 5d13 0000  o........Ord]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 650b 6408 6504 6508 650a 6602 1900 6604  e.d.e.e.e.f...f.
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 4203 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 6b10 0000  o........Krdk...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 6b10 0000  o........Ordk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6501  d.l.m.Z.m.Z...e.
 00000050: 4700 6403 6404 8400 6404 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 4700 6405 6406 8400 6406 8302 5a07 6407  G.d.d...d...Z.d.
 00000070: 5300 2908 e900 0000 0029 02da 0964 6174  S.)......)...dat
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 4178 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 5210 0000  o........KrdR...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 5210 0000  o........OrdR...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6403 6404 6c07 6d08 5a08 0100 6501  ..d.d.l.m.Z...e.
 00000060: 4700 6405 6406 8400 6406 8302 8301 5a09  G.d.d...d.....Z.
 00000070: 4700 6407 6408 8400 6408 8302 5a0a 6409  G.d.d...d...Z.d.
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 9308 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 9308 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6402 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6410 6406 6407 8404 5a0a 6410 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 640a 640b 8400 5a0c 6410 640c  ..Z.d.d...Z.d.d.
@@ -242,16 +242,16 @@
 00000f10: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
 00000f20: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
 00000f30: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
 00000f40: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
 00000f50: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
 00000f60: 7d06 7d05 6400 5300 290d 4e72 0600 0000  }.}.d.S.).Nr....
 00000f70: 7207 0000 0072 0800 0000 720a 0000 003e  r....r....r....>
-00000f80: 0400 0000 7230 0000 0072 2f00 0000 7218  ....r0...r/...r.
-00000f90: 0000 0072 0c00 0000 720e 0000 0029 017a  ...r....r....).z
+00000f80: 0400 0000 7218 0000 0072 0c00 0000 7230  ....r....r....r0
+00000f90: 0000 0072 2f00 0000 720e 0000 0029 017a  ...r/...r....).z
 00000fa0: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
 00000fb0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
 00000fc0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
 00000fd0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
 00000fe0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
 00000ff0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
 00001000: 3029 73da 0373 6574 7224 0000 0029 06da  0)s..setr$...)..
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1442 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 a205 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 a205 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 640c 6406 6407 8404 5a0a 640c 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 640c 640a 640b 8404 5a0c 6401  ..Z.d.d.d...Z.d.
@@ -61,36 +61,36 @@
 000003c0: 6601 6413 7c09 7c0a 6602 a104 7404 a009  f.d.|.|.f...t...
 000003d0: 7c09 a101 7404 a009 7c0a a101 6414 9c02  |...t...|...d...
 000003e0: 1600 7d0b 6415 6416 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
 000003f0: 740a 7404 a00b 7c0c a101 8301 8201 6400  t.t...|.......d.
 00000400: 0400 7d09 0400 7d02 7d0a 6400 5300 2917  ..}...}.}.d.S.).
 00000410: 4efa 1c68 7474 703a 2f2f 6578 616d 706c  N..http://exampl
 00000420: 652e 636f 6d2f 6163 746f 722f 3132 3329  e.com/actor/123)
-00000430: 01da 0269 643e 0500 0000 da05 696e 626f  ...id>......inbo
-00000440: 78da 066f 7574 626f 78da 0474 7970 65fa  x..outbox..type.
-00000450: 0840 636f 6e74 6578 7472 0700 0000 a901  .@contextr......
+00000430: 01da 0269 643e 0500 0000 da06 6f75 7462  ...id>......outb
+00000440: 6f78 da05 696e 626f 78fa 0840 636f 6e74  ox..inbox..@cont
+00000450: 6578 7472 0700 0000 da04 7479 7065 a901  extr......type..
 00000460: fa02 3d3d 2901 7a62 2528 7079 3729 730a  ..==).zb%(py7)s.
 00000470: 7b25 2870 7937 2973 203d 2025 2870 7930  {%(py7)s = %(py0
 00000480: 2973 2825 2870 7935 2973 0a7b 2528 7079  )s(%(py5)s.{%(py
 00000490: 3529 7320 3d20 2528 7079 3329 730a 7b25  5)s = %(py3)s.{%
 000004a0: 2870 7933 2973 203d 2025 2870 7931 2973  (py3)s = %(py1)s
 000004b0: 2e6b 6579 730a 7d28 290a 7d29 0a7d 203d  .keys.}().}).} =
 000004c0: 3d20 2528 7079 3130 2973 da03 7365 74da  = %(py10)s..set.
 000004d0: 0672 6573 756c 7429 06da 0370 7930 da03  .result)...py0..
 000004e0: 7079 31da 0370 7933 da03 7079 35da 0370  py1..py3..py5..p
 000004f0: 7937 da04 7079 3130 7a0f 6173 7365 7274  y7..py10z.assert
 00000500: 2025 2870 7931 3229 73da 0470 7931 327a   %(py12)s..py12z
-00000510: 084a 6f68 6e20 446f 653e 0600 0000 da04  .John Doe>......
-00000520: 6e61 6d65 7208 0000 0072 0900 0000 720a  namer....r....r.
-00000530: 0000 0072 0b00 0000 7207 0000 005a 1130  ...r....r....Z.0
+00000510: 084a 6f68 6e20 446f 653e 0600 0000 720b  .John Doe>....r.
+00000520: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000530: 0000 7207 0000 00da 046e 616d 655a 1130  ..r......nameZ.0
 00000540: 3132 3334 3536 3738 3930 3132 3334 3536  1234567890123456
-00000550: da03 6b65 793e 0700 0000 7217 0000 0072  ..key>....r....r
-00000560: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
-00000570: 0000 0072 0700 0000 da09 7075 626c 6963  ...r......public
-00000580: 4b65 7972 1900 0000 7a04 236b 6579 2903  Keyr....z.#key).
+00000550: da03 6b65 793e 0700 0000 720b 0000 0072  ..key>....r....r
+00000560: 0800 0000 7209 0000 0072 0a00 0000 da09  ....r....r......
+00000570: 7075 626c 6963 4b65 7972 0700 0000 7217  publicKeyr....r.
+00000580: 0000 0072 1900 0000 7a04 236b 6579 2903  ...r....z.#key).
 00000590: 7207 0000 00da 056f 776e 6572 da0c 7075  r......owner..pu
 000005a0: 626c 6963 4b65 7950 656d a901 7a12 2528  blicKeyPem..z.%(
 000005b0: 7079 3129 7320 3d3d 2025 2870 7934 2973  py1)s == %(py4)s
 000005c0: a902 7211 0000 00da 0370 7934 fa0e 6173  ..r......py4..as
 000005d0: 7365 7274 2025 2870 7936 2973 da03 7079  sert %(py6)s..py
 000005e0: 3629 1072 0400 0000 da05 6275 696c 64da  6).r......build.
 000005f0: 046b 6579 7372 0e00 0000 da0a 4070 7974  .keysr......@pyt
@@ -152,17 +152,17 @@
 00000970: 7d01 7c01 640c 1900 640d 1900 7d02 640a  }.|.d...d...}.d.
 00000980: 7d03 7c02 7c03 6b02 7d04 7c04 73b0 7402  }.|.|.k.}.|.s.t.
 00000990: a003 6405 7c04 6601 6406 7c02 7c03 6602  ..d.|.f.d.|.|.f.
 000009a0: a104 7402 a004 7c02 a101 7402 a004 7c03  ..t...|...t...|.
 000009b0: a101 6407 9c02 1600 7d05 6408 6409 7c05  ..d.....}.d.d.|.
 000009c0: 6901 1600 7d06 7405 7402 a006 7c06 a101  i...}.t.t...|...
 000009d0: 8301 8201 6400 0400 7d02 0400 7d04 7d03  ....d...}...}.}.
-000009e0: 6400 5300 290e 4e72 0600 0000 7208 0000  d.S.).Nr....r...
-000009f0: 0072 0900 0000 a903 7207 0000 0072 0800  .r......r....r..
-00000a00: 0000 7209 0000 0072 0c00 0000 721c 0000  ..r....r....r...
+000009e0: 6400 5300 290e 4e72 0600 0000 7209 0000  d.S.).Nr....r...
+000009f0: 0072 0800 0000 a903 7207 0000 0072 0900  .r......r....r..
+00000a00: 0000 7208 0000 0072 0c00 0000 721c 0000  ..r....r....r...
 00000a10: 0072 1d00 0000 721f 0000 0072 2000 0000  .r....r....r ...
 00000a20: 7a18 6874 7470 3a2f 2f65 7861 6d70 6c65  z.http://example
 00000a30: 2e63 6f6d 2f70 726f 7879 2901 da0a 7669  .com/proxy)...vi
 00000a40: 7369 6269 6c69 7479 da09 656e 6470 6f69  sibility..endpoi
 00000a50: 6e74 73da 0870 726f 7879 5572 6c29 0a72  nts..proxyUrl).r
 00000a60: 0400 0000 7221 0000 0072 2300 0000 7224  ....r!...r#...r$
 00000a70: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
@@ -181,16 +181,16 @@
 00000b40: 7d02 6405 6406 6901 7d03 7c02 7c03 6b02  }.d.d.i.}.|.|.k.
 00000b50: 7d04 7c04 7341 7403 a004 6408 7c04 6601  }.|.sAt...d.|.f.
 00000b60: 6409 7c02 7c03 6602 a104 7403 a005 7c02  d.|.|.f...t...|.
 00000b70: a101 7403 a005 7c03 a101 640a 9c02 1600  ..t...|...d.....
 00000b80: 7d05 640b 640c 7c05 6901 1600 7d06 7406  }.d.d.|.i...}.t.
 00000b90: 7403 a007 7c06 a101 8301 8201 6400 0400  t...|.......d...
 00000ba0: 7d02 0400 7d04 7d03 6400 5300 290d 4e72  }...}.}.d.S.).Nr
-00000bb0: 0600 0000 7208 0000 0072 0900 0000 723c  ....r....r....r<
-00000bc0: 0000 0072 0a00 0000 5a05 496d 6167 65da  ...r....Z.Image.
+00000bb0: 0600 0000 7209 0000 0072 0800 0000 723c  ....r....r....r<
+00000bc0: 0000 0072 0b00 0000 5a05 496d 6167 65da  ...r....Z.Image.
 00000bd0: 0469 636f 6e72 0c00 0000 721c 0000 0072  .iconr....r....r
 00000be0: 1d00 0000 721f 0000 0072 2000 0000 2908  ....r....r ...).
 00000bf0: 7204 0000 0072 4400 0000 7221 0000 0072  r....rD...r!...r
 00000c00: 2300 0000 7224 0000 0072 2800 0000 7229  #...r$...r(...r)
 00000c10: 0000 0072 2a00 0000 7242 0000 0072 3900  ...r*...rB...r9.
 00000c20: 0000 7239 0000 0072 3a00 0000 da14 7465  ..r9...r:.....te
 00000c30: 7374 5f61 6374 6f72 5f77 6974 685f 6963  st_actor_with_ic
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1257 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 e904 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 e904 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 640a 6406 6407 8404 5a0a 640a 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 6401 5300 290b e900 0000 004e  ..Z.d.S.)......N
@@ -39,37 +39,37 @@
 00000260: 0474 07a0 0c7c 0aa1 0174 07a0 0c7c 0ba1  .t...|...t...|..
 00000270: 0164 109c 0216 007d 0c64 1164 127c 0c69  .d.....}.d.d.|.i
 00000280: 0116 007d 0d74 0d74 07a0 0e7c 0da1 0183  ...}.t.t...|....
 00000290: 0182 0164 0004 007d 0a04 007d 037d 0b64  ...d...}...}.}.d
 000002a0: 0053 0029 144e da08 6163 746f 725f 6964  .S.).N..actor_id
 000002b0: da09 666f 6c6c 6f77 6572 7329 02da 0269  ..followers)...i
 000002c0: 6472 0700 0000 da04 7465 7874 3e06 0000  dr......text>...
-000002d0: 00da 0263 63da 0474 7970 65da 0c61 7474  ...cc..type..att
-000002e0: 7269 6275 7465 6454 6ffa 0840 636f 6e74  ributedTo..@cont
-000002f0: 6578 74da 0763 6f6e 7465 6e74 da02 746f  ext..content..to
+000002d0: 00fa 0840 636f 6e74 6578 74da 0c61 7474  ...@context..att
+000002e0: 7269 6275 7465 6454 6fda 0274 6fda 0263  ributedTo..to..c
+000002f0: 63da 0474 7970 65da 0763 6f6e 7465 6e74  c..type..content
 00000300: a901 fa02 3d3d a901 7a62 2528 7079 3729  ....==..zb%(py7)
 00000310: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
 00000320: 7930 2973 2825 2870 7935 2973 0a7b 2528  y0)s(%(py5)s.{%(
 00000330: 7079 3529 7320 3d20 2528 7079 3329 730a  py5)s = %(py3)s.
 00000340: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
 00000350: 2973 2e6b 6579 730a 7d28 290a 7d29 0a7d  )s.keys.}().}).}
 00000360: 203d 3d20 2528 7079 3130 2973 da03 7365   == %(py10)s..se
 00000370: 74da 0672 6573 756c 74a9 06da 0370 7930  t..result....py0
 00000380: da03 7079 31da 0370 7933 da03 7079 35da  ..py1..py3..py5.
 00000390: 0370 7937 da04 7079 3130 fa0f 6173 7365  .py7..py10..asse
 000003a0: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
-000003b0: 3272 0f00 0000 7a2c 6874 7470 733a 2f2f  2r....z,https://
+000003b0: 3272 0c00 0000 7a2c 6874 7470 733a 2f2f  2r....z,https://
 000003c0: 7777 772e 7733 2e6f 7267 2f6e 732f 6163  www.w3.org/ns/ac
 000003d0: 7469 7669 7479 7374 7265 616d 7323 5075  tivitystreams#Pu
 000003e0: 626c 6963 a901 7a12 2528 7079 3129 7320  blic..z.%(py1)s 
 000003f0: 3d3d 2025 2870 7934 2973 a902 7217 0000  == %(py4)s..r...
 00000400: 00da 0370 7934 fa0e 6173 7365 7274 2025  ...py4..assert %
-00000410: 2870 7936 2973 da03 7079 3672 0a00 0000  (py6)s..py6r....
+00000410: 2870 7936 2973 da03 7079 3672 0d00 0000  (py6)s..py6r....
 00000420: 290f 7204 0000 00da 046e 6f74 65da 0961  ).r......note..a
-00000430: 735f 7075 626c 6963 720e 0000 00da 0562  s_publicr......b
+00000430: 735f 7075 626c 6963 720f 0000 00da 0562  s_publicr......b
 00000440: 7569 6c64 da04 6b65 7973 7213 0000 00da  uild..keysr.....
 00000450: 0a40 7079 7465 7374 5f61 72da 115f 6361  .@pytest_ar.._ca
 00000460: 6c6c 5f72 6570 7263 6f6d 7061 7265 da0c  ll_reprcompare..
 00000470: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
 00000480: 6361 6c73 da18 5f73 686f 756c 645f 7265  cals.._should_re
 00000490: 7072 5f67 6c6f 6261 6c5f 6e61 6d65 da09  pr_global_name..
 000004a0: 5f73 6166 6572 6570 72da 0e41 7373 6572  _saferepr..Asser
@@ -142,22 +142,22 @@
 000008d0: 6413 6414 7c0e 6901 1600 7d0f 740e 7408  d.d.|.i...}.t.t.
 000008e0: a00f 7c0f a101 8301 8201 6400 0400 7d0c  ..|.......d...}.
 000008f0: 0400 7d05 7d0d 6400 5300 291d 4e7a 1468  ..}.}.d.S.).Nz.h
 00000900: 7474 7073 3a2f 2f72 656d 6f74 652f 616c  ttps://remote/al
 00000910: 6963 657a 2568 7474 7073 3a2f 2f77 7777  icez%https://www
 00000920: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
 00000930: 6974 7973 7472 6561 6d73 da06 5065 7273  itystreams..Pers
-00000940: 6f6e 5a06 616c 7973 7361 2904 720d 0000  onZ.alyssa).r...
-00000950: 0072 0800 0000 720b 0000 00da 1170 7265  .r....r......pre
+00000940: 6f6e 5a06 616c 7973 7361 2904 720a 0000  onZ.alyssa).r...
+00000950: 0072 0800 0000 720e 0000 00da 1170 7265  .r....r......pre
 00000960: 6665 7272 6564 5573 6572 6e61 6d65 2901  ferredUsername).
-00000970: da06 636c 6965 6e74 3e04 0000 00da 046e  ..client>......n
-00000980: 616d 65da 0468 7265 6672 0b00 0000 720d  ame..hrefr....r.
-00000990: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
+00000970: da06 636c 6965 6e74 3e04 0000 0072 0e00  ..client>....r..
+00000980: 0000 da04 6e61 6d65 720a 0000 00da 0468  ....namer......h
+00000990: 7265 6672 1000 0000 7212 0000 0072 1300  refr....r....r..
 000009a0: 0000 da07 6d65 6e74 696f 6e72 1500 0000  ....mentionr....
-000009b0: 721c 0000 0072 1d00 0000 720b 0000 00da  r....r....r.....
+000009b0: 721c 0000 0072 1d00 0000 720e 0000 00da  r....r....r.....
 000009c0: 074d 656e 7469 6f6e 721e 0000 0072 1f00  .Mentionr....r..
 000009d0: 0000 7221 0000 0072 2200 0000 7242 0000  ..r!...r"...rB..
 000009e0: 0029 017a 1225 2870 7931 2973 203d 3d20  .).z.%(py1)s == 
 000009f0: 2528 7079 3329 73da 0a72 656d 6f74 655f  %(py3)s..remote_
 00000a00: 7572 6929 0272 1700 0000 7218 0000 007a  uri).r....r....z
 00000a10: 0e61 7373 6572 7420 2528 7079 3529 7372  .assert %(py5)sr
 00000a20: 1900 0000 7241 0000 007a 0d61 6c79 7373  ....rA...z.alyss
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1034 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 0a04 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 0a04 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 640b 6405 6406 8404 5a08 640b  Z...d.d.d...Z.d.
 00000060: 6407 6408 8404 5a09 640b 6409 640a 8404  d.d...Z.d.d.d...
 00000070: 5a0a 6401 5300 290c e900 0000 004e e901  Z.d.S.)......N..
```

### Comparing `bovine-0.2.3/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 3103 0000  o........Krd1...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 3103 0000  o........Ord1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6407 6405 6406 8404 5a08 6401  Z...d.d.d...Z.d.
 00000060: 5300 2908 e900 0000 004e e901 0000 0029  S.)......N.....)
 00000070: 01da 154f 7264 6572 6564 436f 6c6c 6563  ...OrderedCollec
```

### Comparing `bovine-0.2.3/bovine/activitystreams/activity_factory.py` & `bovine-0.2.4/bovine/activitystreams/activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/object_factory.py` & `bovine-0.2.4/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/test_activity_factory.py` & `bovine-0.2.4/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/test_actor.py` & `bovine-0.2.4/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/test_object_factory.py` & `bovine-0.2.4/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.2.4/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.2.4/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/utils/__init__.py` & `bovine-0.2.4/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.4/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 3209 0000  o........Krd2...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 3209 0000  o........Ord2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6504 6404 6505 6604  m.Z...d.e.d.e.f.
 00000050: 6405 6406 8404 5a06 6403 6501 6504 6505  d.d...Z.d.e.e.e.
 00000060: 4200 1900 6404 6501 6505 1900 6604 6407  B...d.e.e...f.d.
 00000070: 6408 8404 5a07 6409 640a 8400 5a08 6403  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.2.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc` & `bovine-0.2.4/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 865 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 6103 0000  o........Krda...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 6103 0000  o........Orda...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6407  d.l.Z.d.d...Z.d.
 00000040: 6405 6406 8401 5a02 6401 5300 2908 e900  d.d...Z.d.S.)...
 00000050: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0002 0000 0007 0000 0043 0000 0073 6400  .........C...sd.
 00000070: 0000 6401 7c00 7600 7217 7400 6402 7c00  ..d.|.v.r.t.d.|.
```

### Comparing `bovine-0.2.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 da08 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 da08 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6405 6406  Z.m.Z.m.Z...d.d.
 00000070: 8400 5a0d 6407 6408 8400 5a0e 6409 640a  ..Z.d.d...Z.d.d.
@@ -30,19 +30,19 @@
 000001d0: 740d 7407 a00e 7c05 a101 8301 8201 6400  t.t...|.......d.
 000001e0: 0400 7d03 7d02 6400 5300 290f 4eda 044e  ..}.}.d.S.).N..N
 000001f0: 6f74 65da 0761 6363 6f75 6e74 fa11 6163  ote..account..ac
 00000200: 636f 756e 742f 666f 6c6c 6f77 6572 73a9  count/followers.
 00000210: 03da 0474 7970 65da 0d61 7474 7269 6275  ...type..attribu
 00000220: 7465 645f 746f da09 666f 6c6c 6f77 6572  ted_to..follower
 00000230: 73da 0263 63da 0274 6fda 0473 616d 653e  s..cc..to..same>
-00000240: 0500 0000 720a 0000 0072 0f00 0000 7a2c  ....r....r....z,
-00000250: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
-00000260: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
-00000270: 7265 616d 7323 5075 626c 6963 7211 0000  reams#Publicr...
-00000280: 0072 1000 0000 a901 fa02 3d3d 2901 7a12  .r........==).z.
+00000240: 0500 0000 720a 0000 0072 1000 0000 720f  ....r....r....r.
+00000250: 0000 0072 1100 0000 7a2c 6874 7470 733a  ...r....z,https:
+00000260: 2f2f 7777 772e 7733 2e6f 7267 2f6e 732f  //www.w3.org/ns/
+00000270: 6163 7469 7669 7479 7374 7265 616d 7323  activitystreams#
+00000280: 5075 626c 6963 a901 fa02 3d3d 2901 7a12  Public....==).z.
 00000290: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
 000002a0: 2973 da0a 7265 6369 7069 656e 7473 2902  )s..recipients).
 000002b0: da03 7079 30da 0370 7933 7a0e 6173 7365  ..py0..py3z.asse
 000002c0: 7274 2025 2870 7935 2973 da03 7079 3529  rt %(py5)s..py5)
 000002d0: 0f72 0200 0000 da09 6173 5f70 7562 6c69  .r......as_publi
 000002e0: 6372 0f00 0000 da03 6164 6472 1000 0000  cr......addr....
 000002f0: da05 6275 696c 6472 0700 0000 da0a 4070  ..buildr......@p
```

### Comparing `bovine-0.2.3/bovine/activitystreams/utils/print.py` & `bovine-0.2.4/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/activitystreams/utils/test_utils.py` & `bovine-0.2.4/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/__init__.py` & `bovine-0.2.4/bovine/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 3968 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 800f 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 800f 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6404 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/bearer.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/bearer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1794 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 0207 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 0207 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000060: 8400 6407 8302 5a07 6401 5300 2908 e900  ..d...Z.d.S.)...
 00000070: 0000 004e 2901 da0b 6765 745f 676d 745f  ...N)...get_gmt_
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/event_source.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/event_source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1520 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 f005 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 f005 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a05 6402 5300  d.d...d...Z.d.S.
 00000060: 2906 e900 0000 0029 01da 0444 6963 744e  )......)...DictN
 00000070: 2901 da0f 5365 7276 6572 5365 6e74 4576  )...ServerSentEv
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/lookup_account.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 868 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 6403 0000  o........Krdd...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 6403 0000  o........Ordd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6401 5300  e.f.d.d...Z.d.S.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/moo_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 3001 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 b90b 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 b90b 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 8400 5a0c 4700  m.Z...d.d...Z.G.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 b403 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 b403 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6404 6503  e.f.d.d...Z.d.e.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/signed_http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1150 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 7e04 0000  o........Krd~...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 7e04 0000  o........Ord~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 4400 0000 6500  .....@...sD...e.
 00000070: 5a01 6400 5a02 6401 5a03 640d 6403 6404  Z.d.Z.d.Z.d.d.d.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 ce0c 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 ce0c 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 651 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 8b02 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 8b02 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6408 6406 6407 8404 5a0a 6401 5300 2909  d.d.d...Z.d.S.).
 00000070: e900 0000 004e 2901 da09 4173 796e 634d  .....N)...AsyncM
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1505 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 e105 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 e105 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 6d0a  d.d.l.m.Z.m.Z.m.
 00000060: 5a0a 0100 6404 6405 8400 5a0b 6406 6407  Z...d.d...Z.d.d.
 00000070: 8400 5a0c 6408 6409 8400 5a0d 640a 640b  ..Z.d.d...Z.d.d.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 3f01 0000  o........Krd?...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 3f01 0000  o........Ord?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 8400 5a09 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0e66 6574 6368 5f6e  .....)...fetch_n
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 8104 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 8104 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a09  Z.m.Z...d.d.l.Z.
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405 6406  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.2.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 0a02 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 0a02 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a08 6400 6403  Z...d.d.l.Z.d.d.
 00000060: 6c09 6d0a 5a0a 0100 6404 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6406 6407 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
```

### Comparing `bovine-0.2.3/bovine/clients/bearer.py` & `bovine-0.2.4/bovine/clients/bearer.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/event_source.py` & `bovine-0.2.4/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/lookup_account.py` & `bovine-0.2.4/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/moo_auth.py` & `bovine-0.2.4/bovine/clients/moo_auth.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/nodeinfo.py` & `bovine-0.2.4/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/signed_http.py` & `bovine-0.2.4/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/signed_http_methods.py` & `bovine-0.2.4/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/test_event_source.py` & `bovine-0.2.4/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/test_lookup_account.py` & `bovine-0.2.4/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/test_signed_http.py` & `bovine-0.2.4/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/clients/test_signed_http_client.py` & `bovine-0.2.4/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/__init__.py` & `bovine-0.2.4/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 4141 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 2d10 0000  o........Krd-...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 2d10 0000  o........Ord-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6406 6407 6c0c 6d0d 5a0d 6d0e 5a0e  Z.d.d.l.m.Z.m.Z.
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/helper.cpython-310.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2664 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 680a 0000  o........Krdh...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 680a 0000  o........Ordh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/http_signature.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 4008 0000  o........Krd@...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 4008 0000  o........Ord@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6405  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6500 a00c 650d a101 5a0e 6407 6408  ..e...e...Z.d.d.
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 7e0b 0000  o........Krd~...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 7e0b 0000  o........Ord~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c04 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6404 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 f204 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 f204 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 a001 6502 a101 5a03  d.l.Z.e...e...Z.
 00000040: 4700 6402 6403 8400 6403 8302 5a04 6404  G.d.d...d...Z.d.
 00000050: 6405 8400 5a05 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000060: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000070: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 2199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 9708 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 9708 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
 00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
 00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
 00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
 00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 4995 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 8313 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 8313 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
 00000070: 5a0e 0100 6403 6405 6c0f 6d10 5a10 0100  Z...d.d.l.m.Z...
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 8003 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 8003 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6403 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6406 6407  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 5081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 d913 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 d913 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6402 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6402 6405  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6406 6407 8400 5a0e  l.m.Z...d.d...Z.
```

### Comparing `bovine-0.2.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 b704 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 b704 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0953 6967 6e61 7475  .....)...Signatu
```

### Comparing `bovine-0.2.3/bovine/crypto/helper.py` & `bovine-0.2.4/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/http_signature.py` & `bovine-0.2.4/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/signature_checker.py` & `bovine-0.2.4/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/signature_parser.py` & `bovine-0.2.4/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/test.py` & `bovine-0.2.4/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/test_crypto.py` & `bovine-0.2.4/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/test_helper.py` & `bovine-0.2.4/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/test_http_signature.py` & `bovine-0.2.4/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/crypto/test_signature_parser.py` & `bovine-0.2.4/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/jsonld.py` & `bovine-0.2.4/bovine/jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/msg.py` & `bovine-0.2.4/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/repl.py` & `bovine-0.2.4/bovine/repl.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/test_jsonld.py` & `bovine-0.2.4/bovine/test_jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/types.py` & `bovine-0.2.4/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/utils/__init__.py` & `bovine-0.2.4/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.4/bovine/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 856 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 5803 0000  o........KrdX...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 5803 0000  o........OrdX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6505 6404 6505 6405 6505 6406 6506 6608  e.d.e.d.e.d.e.f.
 00000060: 6407 6408 8404 5a07 6409 6505 6406 6504  d.d...Z.d.e.d.e.
 00000070: 6505 6503 6505 1900 6602 1900 6604 640a  e.e.e...f...f.d.
```

### Comparing `bovine-0.2.3/bovine/utils/__pycache__/date.cpython-310.pyc` & `bovine-0.2.4/bovine/utils/__pycache__/date.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 0702 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 0702 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 6d02 5a02  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6505 6602 6404 6405 8404 5a06 6406 6505  e.f.d.d...Z.d.e.
 00000060: 6403 6500 6604 6407 6408 8404 5a07 640f  d.e.f.d.d...Z.d.
 00000070: 640a 6500 640b 6508 6403 6509 6606 640c  d.e.d.e.d.e.f.d.
```

### Comparing `bovine-0.2.3/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc` & `bovine-0.2.4/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 4736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 8012 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 8012 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 6d04 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6401 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6408  m.Z.m.Z.m.Z...d.
 00000070: 6406 6407 8401 5a0c 6402 5300 2909 6178  d.d...Z.d.S.).ax
```

### Comparing `bovine-0.2.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 761 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 f902 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 f902 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100  l.m.Z.m.Z.m.Z...
 00000070: 640c 6406 6407 8404 5a0d 640c 6408 6409  d.d.d...Z.d.d.d.
```

### Comparing `bovine-0.2.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 c401 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 c401 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1670 6172 7365 5f66 6564 6976 6572 7365  .parse_fediverse
```

### Comparing `bovine-0.2.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 7001 0000  o........Krdp...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 7001 0000  o........Ordp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6404 6405 8400 5a0a 6406 6407 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6401 5300 2908 e900 0000 004e e901 0000  d.S.)......N....
```

### Comparing `bovine-0.2.3/bovine/utils/date.py` & `bovine-0.2.4/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/utils/msg/__init__.py` & `bovine-0.2.4/bovine/utils/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.4/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 1432 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 9805 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 9805 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6407 6408 8400 5a09 6409  m.Z...d.d...Z.d.
 00000070: 6500 6a0a 640a 650b 640b 650b 6606 640c  e.j.d.e.d.e.f.d.
```

### Comparing `bovine-0.2.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.4/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 599 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 5702 0000  o........KrdW...
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 5702 0000  o........OrdW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6412 6405 6406 8404 5a0a 6412 6407 6408  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 6506 6a0c a00d 6409 640a 640b  ..Z.e.j...d.d.d.
```

### Comparing `bovine-0.2.3/bovine/utils/msg/__pycache__/validation.cpython-310.pyc` & `bovine-0.2.4/bovine/utils/msg/__pycache__/validation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 27 18:25:16 2023 UTC, .py size: 261 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0c4b 7264 0501 0000  o........Krd....
+00000000: 6f0d 0d0a 0000 0000 f54f 7264 0501 0000  o........Ord....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6500 6401 4200 6602 6402 6403 8404 5a01  e.d.B.f.d.d...Z.
 00000040: 6404 6502 6602 6405 6406 8404 5a03 6401  d.e.f.d.d...Z.d.
 00000050: 5300 2907 da03 746f 734e 6301 0000 0000  S.)...tosNc.....
 00000060: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
 00000070: 0000 0073 1e00 0000 7c00 6400 7500 7206  ...s....|.d.u.r.
```

### Comparing `bovine-0.2.3/bovine/utils/msg/test_validation.py` & `bovine-0.2.4/bovine/utils/msg/test_validation.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/utils/pyld_requests.py` & `bovine-0.2.4/bovine/utils/pyld_requests.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/bovine/utils/test_date.py` & `bovine-0.2.4/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.3/pyproject.toml` & `bovine-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.2.3"
+version = "0.2.4"
 description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
```

### Comparing `bovine-0.2.3/PKG-INFO` & `bovine-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.2.3
+Version: 0.2.4
 Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

