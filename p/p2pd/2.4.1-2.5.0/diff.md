# Comparing `tmp/p2pd-2.4.1.tar.gz` & `tmp/p2pd-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2pd-2.4.1.tar", last modified: Fri May 19 04:39:19 2023, max compression
+gzip compressed data, was "p2pd-2.5.0.tar", last modified: Sun May 28 08:39:20 2023, max compression
```

## Comparing `p2pd-2.4.1.tar` & `p2pd-2.5.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.516197 p2pd-2.4.1/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.4.1/CREDITS.md
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.4.1/LICENSE
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-05-01 10:43:45.000000 p2pd-2.4.1/MANIFEST.in
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-19 04:39:19.516197 p2pd-2.4.1/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-05-01 10:43:45.000000 p2pd-2.4.1/README.md
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.508197 p2pd-2.4.1/p2pd/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/__init__.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/ack_udp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-05-14 07:05:48.000000 p2pd-2.4.1/p2pd/address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30486 2023-04-30 16:44:28.000000 p2pd-2.4.1/p2pd/base_stream.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/cmd_tools.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/echo_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/errors.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5601 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/http_client_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/http_server_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    21525 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5784 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/name_store.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    28663 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23607 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/netiface_extra.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/ntp_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/p2p_node.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.4.1/p2pd/p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.4.1/p2pd/p2p_protocol.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3072 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/p2p_utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/rest_api.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7678 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/settings.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    42083 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    41037 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4766 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/test_init.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17104 2023-05-01 10:43:45.000000 p2pd-2.4.1/p2pd/turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/turn_defs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/turn_process.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/upnp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16346 2023-05-19 04:37:59.000000 p2pd-2.4.1/p2pd/utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/var_names.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/win_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.4.1/p2pd/win_netifaces.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.512197 p2pd-2.4.1/p2pd.egg-info/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1529 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/SOURCES.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/dependency_links.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      110 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/requires.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-05-19 04:39:19.000000 p2pd-2.4.1/p2pd.egg-info/top_level.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      328 2023-05-19 04:37:59.000000 p2pd-2.4.1/requirements.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-05-19 04:39:19.516197 p2pd-2.4.1/setup.cfg
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-05-19 04:37:59.000000 p2pd-2.4.1/setup.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-19 04:39:19.516197 p2pd-2.4.1/tests/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_bind.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_cmd.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2793 2023-05-01 10:43:45.000000 p2pd-2.4.1/tests/test_net_afs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9769 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_p2pd_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1258 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_py_examples.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_rudp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1443 2023-05-01 10:43:45.000000 p2pd-2.4.1/tests/test_signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2197 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_sock.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_sorted_search.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3355 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5614 2023-05-01 10:43:45.000000 p2pd-2.4.1/tests/test_tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6770 2023-05-19 04:37:59.000000 p2pd-2.4.1/tests/test_turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.4.1/tests/test_win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.539903 p2pd-2.5.0/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.5.0/CREDITS.md
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.5.0/LICENSE
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-05-01 10:43:45.000000 p2pd-2.5.0/MANIFEST.in
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-28 08:39:20.539903 p2pd-2.5.0/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-05-01 10:43:45.000000 p2pd-2.5.0/README.md
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.531903 p2pd-2.5.0/p2pd/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/__init__.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/ack_udp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30620 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/base_stream.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/cmd_tools.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/echo_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/errors.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5601 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/http_client_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/http_server_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    22201 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5784 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/name_store.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    29608 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9208 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/nat_test.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23607 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/netiface_extra.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/ntp_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/p2p_node.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.5.0/p2pd/p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.5.0/p2pd/p2p_protocol.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3072 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/p2p_utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/rest_api.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11156 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/settings.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    28879 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    41037 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4766 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/test_init.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17104 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/turn_defs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/turn_process.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/upnp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16417 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/var_names.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/win_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.535903 p2pd-2.5.0/p2pd.egg-info/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1548 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      110 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/requires.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/top_level.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      328 2023-05-19 04:37:59.000000 p2pd-2.5.0/requirements.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-05-28 08:39:20.539903 p2pd-2.5.0/setup.cfg
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-05-28 08:34:04.000000 p2pd-2.5.0/setup.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.539903 p2pd-2.5.0/tests/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_bind.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_cmd.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2793 2023-05-01 10:43:45.000000 p2pd-2.5.0/tests/test_net_afs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9769 2023-05-19 04:37:59.000000 p2pd-2.5.0/tests/test_p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_p2pd_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1258 2023-05-19 04:37:59.000000 p2pd-2.5.0/tests/test_py_examples.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_rudp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1443 2023-05-01 10:43:45.000000 p2pd-2.5.0/tests/test_signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2342 2023-05-28 08:34:04.000000 p2pd-2.5.0/tests/test_sock.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_sorted_search.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3385 2023-05-28 08:34:04.000000 p2pd-2.5.0/tests/test_stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5614 2023-05-01 10:43:45.000000 p2pd-2.5.0/tests/test_tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6770 2023-05-19 04:37:59.000000 p2pd-2.5.0/tests/test_turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_win_netifaces.py
```

### Comparing `p2pd-2.4.1/CREDITS.md` & `p2pd-2.5.0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/LICENSE` & `p2pd-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/PKG-INFO` & `p2pd-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.4.1
+Version: 2.5.0
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.4.1/README.md` & `p2pd-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/__init__.py` & `p2pd-2.5.0/p2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/ack_udp.py` & `p2pd-2.5.0/p2pd/ack_udp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/address.py` & `p2pd-2.5.0/p2pd/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import socket
 import ipaddress
 from .net import *
 
 # TODO: address doesn't support domain resolution
 # from a specific interface. This may not matter though.
 class Address():
-    def __init__(self, host, port, route, sock_type=socket.SOCK_STREAM, timeout=1):
+    def __init__(self, host, port, route, sock_type=socket.SOCK_STREAM, timeout=2):
         self.timeout = timeout
         self.resolved = False
         self.sock_type = sock_type
         self.route = route
         self.host = host
         self.host_type = None
         self.port = int(port)
```

### Comparing `p2pd-2.4.1/p2pd/base_stream.py` & `p2pd-2.5.0/p2pd/base_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                 q.get_nowait()
 
             # Put an item on the queue.
             assert(isinstance(client_tup, tuple))
             q.put_nowait([client_tup, data])
 
         # Apply bool filters to message.
+        msg_added = False
         client_addr = b"%s:%d" % (to_b(client_tup[0]), client_tup[1])
         for sub, q, handler in self.subs.values():
             # Msg pattern, address pattern.
             b_msg_p, b_addr_p = sub
 
             # Check client_addr matches their host pattern.
             if b_addr_p:
@@ -125,16 +126,20 @@
             # Execute message using handle instead of adding to queue.
             if handler is not None:
                 log("handler not none.")
                 run_handler(self.proto, handler, client_tup, data)
                 continue
 
             # Add message to queue.
+            msg_added = True
             do_add(q)
 
+        if not msg_added:
+            log(f"Discarded {client_tup} = {data}")
+
     # Async wait for a message that matches a pattern in a queue.
     async def recv(self, sub=SUB_ALL, timeout=2, full=False):
         recv_timeout = timeout or self.conf["recv_timeout"]
         offset = self.hash_sub(sub)
         try:
             # Sanity checking.
             if offset not in self.subs:
```

### Comparing `p2pd-2.4.1/p2pd/clock_skew.py` & `p2pd-2.5.0/p2pd/clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/cmd_tools.py` & `p2pd-2.5.0/p2pd/cmd_tools.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/daemon.py` & `p2pd-2.5.0/p2pd/daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/http_client_lib.py` & `p2pd-2.5.0/p2pd/http_client_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/http_server_lib.py` & `p2pd-2.5.0/p2pd/http_server_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/interface.py` & `p2pd-2.5.0/p2pd/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -369,30 +369,48 @@
 
     def set_nat(self, nat):
         assert(isinstance(nat, dict))
         assert(nat.keys() == nat_info().keys())
         self.nat = nat
 
     async def load_nat(self):
-        from .stun_client import STUNClient
+        # Try to avoid circular imports.
+        from .base_stream import pipe_open
+        from .stun_client import STUNClient, STUN_CONF
+        from .nat_test import fast_nat_test
         
-        # Prefer IP4 if available.
-        af = IP4
-        if af not in self.supported():
-            af = IP6
-
-        # STUN is used to test the NAT.
-        stun_client = STUNClient(
-            self,
-            af
-        )
+        # IPv6 only has no NAT!
+        if IP4 not in self.supported():
+            nat = nat_info(OPEN_INTERNET, EQUAL_DELTA)
+        else:
+            # STUN is used to get the delta type.
+            af = IP4
+            stun_client = STUNClient(
+                self,
+                af
+            )
+
+            # Get the NAT type.
+            route = await self.route(af).bind()
+            pipe = await pipe_open(UDP, route=route, conf=STUN_CONF)
+
+            # Run delta test.
+            nat_type, delta = await asyncio.wait_for(
+                asyncio.gather(*[
+                    fast_nat_test(pipe, STUND_SERVERS[af]),
+                    delta_test(stun_client)
+                ]),
+                timeout=2
+            )
+
+            nat = nat_info(nat_type, delta)
+            await pipe.close()
 
         # Load NAT type and delta info.
         # On a server should be open.
-        nat = await stun_client.get_nat_info()
         self.set_nat(nat)
         return nat
 
     def get_scope_id(self):
         assert(self.resolved)
 
         # Interface specified by no on windows.
```

### Comparing `p2pd-2.4.1/p2pd/ip_range.py` & `p2pd-2.5.0/p2pd/ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/name_store.py` & `p2pd-2.5.0/p2pd/name_store.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/nat.py` & `p2pd-2.5.0/p2pd/nat.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,23 @@
                         do_retry = 1
                         break
 
             return new_start_port
 
     # Create a list of tasks to get a mapping for a port range.
     def get_port_tests(start_port, port_dist=1):
+        # Single concurrent STUN req.
+        conf = dict_merge(NET_CONF, {
+            "packet_retry": 1,
+            "retry_no": 1,
+            "recv_timeout": 0.5,
+            "addr_retry": 1,
+            "dns_timeout": 0.5
+        })
+
         # Return task list for tests.
         tasks = []
         for i in range(0, test_no):
             # If start is defined then calculate a list of ports.
             # Otherwise the OS assigns an unused port.
             if start_port:
                 src_port = start_port + (i * port_dist)
@@ -282,22 +291,30 @@
                     raise Exception("src less than 4k in mapping behavior.")
 
                 # Get mapping using specific source port.
                 _, s, local, mapped, _, _ = await stun_client.get_mapping(
                     proto,
                     do_close=0,
                     source_port=src_port,
-                    group=group
+                    group=group,
+                    conf=conf
                 )
 
                 # Return mapping results.
                 return [local, mapped, s]
 
             # Allow for tests to be done concurrently.
-            tasks.append(result_wrapper(src_port))
+            tasks.append(
+                async_wrap_errors(
+                    asyncio.wait_for(
+                        result_wrapper(src_port),
+                        0.5
+                    )
+                )
+            )
 
         return tasks
 
     def get_delta_value(delta_no, dist_no, local_dist, preserv_dist, results):
         for i in range(0, len(results)):
             # Unpack result.
             local, mapped, s = results[i]
@@ -827,9 +844,26 @@
     for k in ["local"]:
         for p in map_info[k]:
             if p <= 1024:
                 error = f"invalid low port found for mapping {p}"
                 log(error)
                 raise Exception(error)
 
+async def nat_predict_main():
+    from .stun_client import STUNClient
+    from .interface import Interface, init_p2pd
+
+    # Load default interface.
+    netifaces = await init_p2pd()
+    i = await Interface(netifaces=netifaces).start_local()
+    s = STUNClient(i)
+    
+    # Run delta test and profile it.
+    s1 = timestamp(1)
+    out = await delta_test(s)
+    print(f"delta test time = {timestamp(1) - s1}")
+    print(out)
 
+    # 0.36
 
+if __name__ == "__main__":
+    async_test(nat_predict_main)
```

### Comparing `p2pd-2.4.1/p2pd/net.py` & `p2pd-2.5.0/p2pd/net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/netiface_extra.py` & `p2pd-2.5.0/p2pd/netiface_extra.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/ntp_client.py` & `p2pd-2.5.0/p2pd/ntp_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/p2p_addr.py` & `p2pd-2.5.0/p2pd/p2p_addr.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/p2p_node.py` & `p2pd-2.5.0/p2pd/p2p_node.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/p2p_pipe.py` & `p2pd-2.5.0/p2pd/p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/p2p_protocol.py` & `p2pd-2.5.0/p2pd/p2p_protocol.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/p2p_utils.py` & `p2pd-2.5.0/p2pd/p2p_utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/rest_api.py` & `p2pd-2.5.0/p2pd/rest_api.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/route.py` & `p2pd-2.5.0/p2pd/route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/route_table.py` & `p2pd-2.5.0/p2pd/route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/signaling.py` & `p2pd-2.5.0/p2pd/signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/stun_client.py` & `p2pd-2.5.0/p2pd/stun_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -86,58 +86,14 @@
     # many times to retry the whole thing.
     "retry_no": 3,
 
     # Reuse address tuple for bind() socket call.
     "reuse_addr": True,
 }, NET_CONF)
 
-# Replace with servers from settings.
-# Remove distinction between 'map' and 'change' servers.
-# Just keep change servers to keep things simple.
-STUN_SERVERS_MAP_UDP_V6 = [STUND_SERVERS[IP6][0]] + shuffle(STUND_SERVERS[IP6][1:])
-STUN_SERVERS_CHANGE_UDP_V6 = [STUND_SERVERS[IP6][0]] + shuffle(STUND_SERVERS[IP6][1:])
-STUN_SERVERS_MAP_UDP_V4 = [STUND_SERVERS[IP4][0]] + shuffle(STUND_SERVERS[IP4][1:])
-STUN_SERVERS_CHANGE_UDP_V4 = [STUND_SERVERS[IP4][0]] + shuffle(STUND_SERVERS[IP4][1:])
-STUN_SERVERS_MAP_TCP_V6 = [STUNT_SERVERS[IP6][0]] + shuffle(STUNT_SERVERS[IP6][1:])
-STUN_SERVERS_CHANGE_TCP_V6 = [STUNT_SERVERS[IP6][0]] + shuffle(STUNT_SERVERS[IP6][1:])
-STUN_SERVERS_MAP_TCP_V4 = [STUNT_SERVERS[IP4][0]] + shuffle(STUNT_SERVERS[IP4][1:])
-STUN_SERVERS_CHANGE_TCP_V4 = [STUNT_SERVERS[IP4][0]] + shuffle(STUNT_SERVERS[IP4][1:])
-
-# Apply funcs easier to all server lists.
-STUN_SERVERS = [
-    STUN_SERVERS_MAP_UDP_V4, STUN_SERVERS_MAP_UDP_V6,
-    STUN_SERVERS_MAP_TCP_V4, STUN_SERVERS_MAP_TCP_V6,
-    STUN_SERVERS_CHANGE_UDP_V4, STUN_SERVERS_CHANGE_UDP_V6,
-    STUN_SERVERS_CHANGE_TCP_V4, STUN_SERVERS_CHANGE_TCP_V6,
-]
-
-# Return stun server list easily.
-STUN_SERVER_INDEX = {
-    "change": {
-        socket.SOCK_DGRAM: {
-            socket.AF_INET: STUN_SERVERS_CHANGE_UDP_V4,
-            socket.AF_INET6: STUN_SERVERS_CHANGE_UDP_V6
-        },
-        socket.SOCK_STREAM: {
-            socket.AF_INET: STUN_SERVERS_CHANGE_TCP_V4,
-            socket.AF_INET6: STUN_SERVERS_CHANGE_TCP_V6
-        }
-    },
-    "map": {
-        socket.SOCK_DGRAM: {
-            socket.AF_INET: STUN_SERVERS_MAP_UDP_V4,
-            socket.AF_INET6: STUN_SERVERS_MAP_UDP_V6
-        },
-        socket.SOCK_STREAM: {
-            socket.AF_INET: STUN_SERVERS_MAP_TCP_V4,
-            socket.AF_INET6: STUN_SERVERS_MAP_TCP_V6
-        }
-    }
-}
-
 # stun consts
 MappedAddress = '0001'
 SourceAddress = '0004'
 ChangedAddress = '0005'
 ChangeRequest = '0003'
 BindRequestMsg = '0001'
 dictValToMsgType = {"0101": "BindResponseMsg"}
@@ -149,25 +105,21 @@
 changeRequest = ''.join(
     [ChangeRequest, '0004', "00000006"]
 )
 changePortRequest = ''.join(
     [ChangeRequest, '0004', "00000002"]
 )
 
-# There are two groups of servers - change and map.
-# change means it supports nat testing.
-# map means it only supports standard bind requests.
-# Servers are further divided by protocol (dgram or stream)
-# and by IP type = ipv4 or ipv6.
-def get_stun_servers(af, proto=socket.SOCK_DGRAM, group="change", do_shuffle=0):
-    servers = STUN_SERVER_INDEX[group][proto][af][:]
-    if do_shuffle:
-        random.shuffle(servers)
+def get_stun_servers(af, proto):
+    if proto == UDP:
+        servers = STUND_SERVERS
+    else:
+        servers = STUNT_SERVERS
 
-    return servers
+    return servers[af]
 
 # Make a random transaction ID -- using in bind requests.
 # Kind of like a poor-mans sequence number for UDP packets.
 # Not that useful when TCP is used with the servers.
 def gen_tran_id():
     return rand_b(16)
 
@@ -308,14 +260,15 @@
 
         # IP server will send change requests from.
         'cip': None,
 
         # Port server will send change requests from.
         'cport': None
     }
+    #print(ret)
 
     # Sanity checking.
     if pipe is None:
         log("> STUN skipping get nat port mapping - s = None")
         return ret
 
     # Init values.
@@ -554,259 +507,14 @@
             tran_info,
             extra,
             changed_addr=changed,
             conf=conf
         )
     ), pipe
 
-"""
-Does multiple sub tests to determine NAT type.
-It will differ dest ips, reply ips and/or reply ports.
-Reply success or failure + external ports reported
-by servers are used to infer the type of NAT.
-Note: complete resolution of NAT type is only
-possible with proto = SOCK_DGRAM. This is because
-the router doesn't just allow inbound connects
-that either haven't been forwarded or
-contacted specifically.
-"""
-async def do_nat_test(stun_addr, interface, af=IP4, proto=UDP, group="change", do_close=1, conf=STUN_CONF):
-    # Important vars / init.
-    test = {} # test[test_no] = test result
-    source_port = 0
-    pipe_list = []
-
-    # Log errors, cleanup and retry.
-    async def handle_error(msg, pipe_list, do_close=1):
-        log("> STUN handle = %s" % (to_s(msg)))
-
-        # Cleanup socket.
-        if do_close:
-            for pipe in pipe_list:
-                if pipe is not None:
-                    await pipe.close()
-
-        # Error -- stun server failed.
-        return [], None, None
-
-    # Helper function to run a nat test.
-    async def run_nat_test(pipe, nat_test, tran_info, conf):
-        test_name, log_msg, dest_addr, test_addr, extra = nat_test
-        ret, pipe = await stun_sub_test(
-            log_msg,
-            dest_addr,
-            interface,
-            af,
-            proto,
-            source_port,
-            test_addr,
-            extra,
-            pipe=pipe,
-            tran_info=tran_info,
-            conf=conf
-        )
-
-        return [test_name, ret, pipe]
-
-    # Do first NAT test.
-    _, test[1], pipe = await run_nat_test(None, [
-            1,
-            "doing first nat test",
-            stun_addr,
-            stun_addr,
-            ""
-        ],
-        tran_info_patterns(stun_addr.tup),
-        conf
-    )
-    
-    # Check first reply.
-    error = stun_check_reply(stun_addr, test[1])
-    if error or pipe is None:
-        return await handle_error("invalid stun reply = %s" % (error), pipe_list)
-    else:
-        source_port = pipe.route.bind_port
-        pipe_list.append(pipe)
-
-    # Log changed port.
-    log(
-        "> STUN changed port = %d, stun port = %d" % (
-            test[1]['cport'],
-            stun_addr.port
-        )
-    )
-    log(
-        "> STUN t1 changed ip = %s" % (
-            test[1]['cip']
-        )
-    )
-
-    # List of nat tests to perform concurrently.
-    # ID, log msg, dest addr, resp addr, extra req data.
-    assert(stun_addr.tup[0] != test[1]['cip'])
-    assert(stun_addr.tup[1] != test[1]['cport'])
-    route = interface.route(af)
-    nat_tests = [
-        [
-            2,
-            "doing NAT test 2 - change req",
-            stun_addr,
-            await Address(
-                test[1]['cip'],
-                test[1]['cport'],
-                route,
-                proto
-            ).res(),
-            changeRequest
-        ],
-        [
-            3,
-            "doing NAT test 3 - to changed addr - reply expected",
-            await Address(
-                test[1]['cip'],
-                stun_addr.port,
-                route,
-                proto
-            ).res(),
-            await Address(
-                test[1]['cip'],
-                stun_addr.port,
-                route,
-                proto
-            ).res(),
-            ""
-        ],
-        [
-            4,
-            "nat test 4",
-            await Address(
-                test[1]['cip'],
-                stun_addr.port,
-                route,
-                proto
-            ).res(),
-            await Address(
-                test[1]['cip'],
-                test[1]['cport'],
-                route,
-                proto
-            ).res(),
-            changePortRequest
-        ]
-    ]
-
-    # Schedule nat tests to run concurrently.
-    tasks = []
-    results = []
-    for i, nat_test in enumerate(nat_tests):
-        # Subscribe to certain messages.
-        tran_info = tran_info_patterns(nat_test[3].tup)
-        pipe.subscribe(tran_info[0:2])
-
-        # Record the NAT test.
-        tasks.append(run_nat_test(pipe, nat_test, tran_info, conf))
-
-    # Check results and index them.
-    results = await asyncio.gather(*tasks)
-    for result in results:
-        result_name, result_ret, _ = result
-        if result_ret is None:
-            return await handle_error("STUN %s failed" % (result_name), pipe_list)
-
-        test[result_name] = result_ret
-
-    # Used later on for nat test 3 code
-    # The fields may not be set if there was no response.
-    if test[1]['rip'] is None or test[3]['rip'] is None:
-        return await handle_error("STUN rip missing", pipe_list)
-    else:
-        ip_check = ip_f(test[1]['rip']) == ip_f(test[3]['rip'])
-        log("> STUN t1 rip = {} t3 rip = {}".format(
-            test[1]['rip'],
-            test[3]['rip']
-        ))
-    port_check = test[1]['rport'] == test[3]['rport']
-    test3_dest = nat_tests[1][2]
-    error = stun_check_reply(test3_dest, test[3])
-    log("> STUN t1 rport = {} t3 rport = {}".format(
-        test[1]['rport'],
-        test[3]['rport']
-    ))
-    log("> STUN t2 resp = {}".format(test[2]['resp']))
-
-
-    # Our local bind addr was equal to external address.
-    # Server is directly open to internet.
-    # TODO: this may be invalid?
-    source_ip = pipe.route.bind_ip()
-    log("> STUN source ip = {}".format(source_ip))
-    if ip_f(test[1]['rip']) == ip_f(source_ip):
-        if test[2]['resp']:
-            # Got a reply back = completely open.
-            log("> STUN open internet detected")
-            typ = OPEN_INTERNET
-        else:
-            # Something is filtering replies.
-            log("> STUN firewall detected")
-            test[1]["resp"] = False
-            typ = SYMMETRIC_UDP_FIREWALL
-    else:
-        # Got a reply from a different IP.
-        # NAT opens mapping for source ip and port
-        # Open to any remote host
-        if test[2]['resp']:
-            """
-            It should be noted that a NAT that preserves the source port
-            will also give a positive for this test though it may not
-            be a full code NAT in reality. Preserving type NATs are
-            accounted for in the mapping behaviour tests though.
-            """
-            log("> STUN full cone detected")
-            typ = FULL_CONE
-        else:
-            # We're sending to the servers
-            # advertised 'change address'
-            # or its second address.
-            # We should be able to get a reply.
-            if error:
-                # Exception -- replies should be possible to receive if we send.
-                return await handle_error("invalid stun reply = %s" % (error), pipe_list)
-            else:
-                # NAT reuses port mappings based on source ip and port.
-                # These conditions apply to test 3.
-                if ip_check and port_check:
-                    # Check results.
-                    if test[4]['resp']:
-                        # NAT reuses port mappings based on src ip and port
-                        # dest host most be white listed and can send from any port.
-                        log("> STUN restrict nat detected")
-                        typ = RESTRICT_NAT
-                    else:
-                        # NAT reuses mappings based on src ip and port
-                        # Dest host must be white listed and send from same port.
-                        log("> STUN restricted port detected")
-                        test[1]['resp'] = False
-                        typ = RESTRICT_PORT_NAT
-                else:
-                    # NAT maps different external ports based on outgoing host.
-                    log("> STUN symmetric nat detected")
-                    typ = SYMMETRIC_NAT
-
-    # Port mappings may still be predictable if NAT
-    # Uses an increasing delta value for successive cons
-    # Simultaneous open will test this.
-    # Note: SymmetricNAT, SymmetricUDPFirewall
-    pipe_list, _, _ = await handle_error(
-        "stun test success",
-        pipe_list,
-        do_close
-    )
-
-    return pipe_list, typ, test[1]
-
 # Basic interface to the most useful functions.
 class STUNClient():
     def __init__(self, interface, af=IP4, sock_timeout=2, consensus=[1, 1], proto=UDP):
         self.interface = interface
         self.af = af
         self.proto = proto
         self.sock_timeout = sock_timeout
@@ -828,40 +536,38 @@
     you won't know straight away if it works.
 
     Fast fail uses TCP and will fail immediately if it can't
     do N connections in a row to different servers. This is
     very useful for rapidly determining whether an interface
     is routable via a certain 'address type'.
     """
-    async def _get_field(self, name, af, proto, interface, source_port=0, group="map", alt_port=0, do_close=0, fast_fail=0, servers=None, local_addr=None, conf=STUN_CONF):
+    async def _get_field(self, name, af, proto, interface, source_port=0, group="map", do_close=0, fast_fail=0, servers=None, local_addr=None, conf=STUN_CONF):
         # Record start time and define fail result funv.
         random.seed()
         start_time = time.time()
         f_fail = lambda: [None, None, time.time() - start_time]
         use_proto = TCP if fast_fail else proto
         lax = 0 if group == "change" else 1
 
+
         # Limit at 20 to avoid massive delays.
         # If 20 consecutive servers fail
         # something else is wrong.
-        servers = servers or get_stun_servers(af, proto, group)
+        servers = servers or get_stun_servers(af, proto)
         stun_addr = None
         for server in servers:
             for i in range(conf["retry_no"]):
                 # Get a valid STUN Address.
                 for j in range(conf["addr_retry"]):
-                    # Basic server address check.
-                    stun_port = 3479 if alt_port else server[1]
-
                     # Resolve address with a timeout.
                     try:
                         stun_addr = await asyncio.wait_for(
                             stun_check_addr_info(
-                                server[0],
-                                stun_port,
+                                server["primary"]["ip"],
+                                server["primary"]["port"],
                                 af,
                                 proto,
                                 interface,
                                 local_addr
                             ),
                             conf["dns_timeout"]
                         )
@@ -926,93 +632,14 @@
                         continue
                     else:
                         return nat_info[name], pipe, stop_time
 
         # Retry failed.
         return f_fail()
 
-    async def get_nat_type(self, af=None, servers=None):
-        if self.proto != UDP:
-            raise Exception("NAT type test requires udp proto.")
-
-        # Setup conf for NAT type.
-        conf = copy.deepcopy(STUN_CONF)
-        conf["packet_retry"] = 3
-        #conf["recv_timeout"] = 4
-        conf["addr_retry"] = 6
-        #conf["retry_no"] = 3
-        #conf["consensus"] = [3, 5]
-
-        # Main function defaults.
-        interface = self.interface
-        threshold_n = conf["consensus"][0] or self.n
-        threshold_t = conf["consensus"][1] or self.t
-        group = "change"
-        af = af or self.af
-        servers = servers or get_stun_servers(
-            af,
-            self.proto,
-            group,
-            0
-        )
-
-        # Do NAT test with retry.
-        async def nat_test_with_retry(servers, interface, conf):
-            # Try find a valid STUN server -- max 20 rand attempts.
-            random.seed()
-            stun_addr = None
-            for j in range(conf["retry_no"]):
-                for i in range(conf["addr_retry"]):
-                    server = random.choice(servers)
-                    try:
-                        stun_addr = await asyncio.wait_for(
-                            stun_check_addr_info(
-                                server[0],
-                                server[1],
-                                af,
-                                self.proto,
-                                interface
-                            ),
-                            conf["dns_timeout"]
-                        )
-                        break
-                    except asyncio.TimeoutError:
-                        stun_addr = None
-                        continue
-
-                # Check it was set or skip this test.
-                if stun_addr is None:
-                    continue
-
-                # Do the nat test.
-                ret = await do_nat_test(
-                    stun_addr,
-                    self.interface,
-                    af,
-                    self.proto,
-                    group,
-                    do_close=1,
-                    conf=conf
-                )
-
-                if ret[1] is not None:
-                    return ret
-
-        # Make list of tests for getting NAT type.
-        tasks = []
-        for i in range(threshold_n):
-            # Go ahead and use that STUN addr for the test.
-            tasks.append(
-                nat_test_with_retry(servers, interface, conf)
-            )
-
-        # Return threshold results.
-        f_filter = lambda r: [x[1] for x in r if isinstance(x[1], int)]
-        return await threshold_gather(tasks, f_filter, threshold_t)
-
     async def get_wan_ip(self, af=None, interface=None, fast_fail=0, servers=None, local_addr=None, conf=STUN_CONF):
         # Defaults.
         af = af or self.af
         interface = interface or self.interface
         group = "map"
 
         # sock_timeout + interface added to be compatible
@@ -1035,44 +662,33 @@
             return ip_norm(wan_ip)
 
     """
     Coming to consensus from multiple STUN results is not supported for
     get_mapping as it is expected for there to be differences in
     successive mappings as part of how NATs work.
     """
-    async def get_mapping(self, proto, af=None, source_port=0, group="map", alt_port=0, do_close=0, fast_fail=0, servers=None, conf=STUN_CONF):
+    async def get_mapping(self, proto, af=None, source_port=0, group="map", do_close=0, fast_fail=0, servers=None, conf=STUN_CONF):
         # Defaults.
         af = af or self.af
         log("> stun mapping for proto = %d; af = %d" % (proto, af))
 
         # Get port mapping from first working server.
         interface = self.interface
-        nat_info, s, run_time = await self._get_field("nat_info", af, proto, interface, source_port, group, alt_port, do_close, fast_fail, servers=servers, conf=conf)
+        nat_info, s, run_time = await self._get_field("nat_info", af, proto, interface, source_port, group, do_close, fast_fail, servers=servers, conf=conf)
         if nat_info is None:
             return [None, None, None, None, None, None]
 
         # Return mapping section of STUN reply.
         local = nat_info["lport"] or source_port
         mapped = nat_info["rport"]
         rip = nat_info["rip"]
         if mapped:
             mapped = int(mapped)
 
         return [interface, s, local, mapped, rip, run_time]
-
-    async def get_nat_info(self):
-        nat_type = await self.get_nat_type()
-
-        # Delta not applicable for some NAT types.
-        if nat_type == OPEN_INTERNET:
-            delta = delta_info(NA_DELTA, 0)
-        else:
-            delta = await delta_test(self)
-            
-        return nat_info(nat_type, delta)
     
 #######################################################################
 if __name__ == "__main__": # pragma: no cover
     """
     Some custom STUN servers don't include the rip attribute
     for change requests -- in this case we issue get_wan_ips
     to both test addresses and use the result for the tests.
@@ -1187,18 +803,21 @@
         server = ['stun.innovaphone.com', 3478]
 
         netifaces = await init_p2pd()
 
 
         i = await Interface().start_local()
         s = STUNClient(interface=i, proto=UDP)
-        out = await s.get_nat_type()
-        print(out)
+        x = await s.get_wan_ip()
+        print(x)
+        return
+
         out = await s.get_mapping(proto=TCP)
         print(out)
+        return
 
         i = await Interface().start()
         print(i)
 
         return
```

### Comparing `p2pd-2.4.1/p2pd/tcp_punch.py` & `p2pd-2.5.0/p2pd/tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/test_init.py` & `p2pd-2.5.0/p2pd/test_init.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/turn_client.py` & `p2pd-2.5.0/p2pd/turn_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/turn_defs.py` & `p2pd-2.5.0/p2pd/turn_defs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/turn_process.py` & `p2pd-2.5.0/p2pd/turn_process.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/upnp.py` & `p2pd-2.5.0/p2pd/upnp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/utils.py` & `p2pd-2.5.0/p2pd/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,14 +489,18 @@
                     loop.close()
 
             loop = asyncio.get_event_loop()
             return loop.run_in_executor(None, helper)
 
     return inner
 
+def cancel_tasks(tasks):
+    for task in tasks:
+        task.cancel()
+
 # Wait for tasks to finish up until a timeout.
 # Otherwise cancel them and wait for errors.
 async def gather_or_cancel(tasks, timeout):
     group_task = asyncio.gather(*tasks)
     try:
         await asyncio.wait_for(
             group_task,
```

### Comparing `p2pd-2.4.1/p2pd/var_names.py` & `p2pd-2.5.0/p2pd/var_names.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/win_net.py` & `p2pd-2.5.0/p2pd/win_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd/win_netifaces.py` & `p2pd-2.5.0/p2pd/win_netifaces.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/p2pd.egg-info/PKG-INFO` & `p2pd-2.5.0/p2pd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.4.1
+Version: 2.5.0
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.4.1/p2pd.egg-info/SOURCES.txt` & `p2pd-2.5.0/p2pd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ./p2pd/errors.py
 ./p2pd/http_client_lib.py
 ./p2pd/http_server_lib.py
 ./p2pd/interface.py
 ./p2pd/ip_range.py
 ./p2pd/name_store.py
 ./p2pd/nat.py
+./p2pd/nat_test.py
 ./p2pd/net.py
 ./p2pd/netiface_extra.py
 ./p2pd/ntp_client.py
 ./p2pd/p2p_addr.py
 ./p2pd/p2p_node.py
 ./p2pd/p2p_pipe.py
 ./p2pd/p2p_protocol.py
```

### Comparing `p2pd-2.4.1/setup.py` & `p2pd-2.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_reqs = f.read().splitlines()
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='2.4.1',
+    version='2.5.0',
     name='p2pd',
     description='Asynchronous P2P networking library and service',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, STUN, TURN, SIP, DHCP, add IP to interface, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='http://github.com/robertsdotpm/p2pd',
     author='Matthew Roberts',
```

### Comparing `p2pd-2.4.1/tests/test_address.py` & `p2pd-2.5.0/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_bind.py` & `p2pd-2.5.0/tests/test_bind.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_clock_skew.py` & `p2pd-2.5.0/tests/test_clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_cmd.py` & `p2pd-2.5.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_daemon.py` & `p2pd-2.5.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_interface.py` & `p2pd-2.5.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_ip_range.py` & `p2pd-2.5.0/tests/test_ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_nat.py` & `p2pd-2.5.0/tests/test_nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_net.py` & `p2pd-2.5.0/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_net_afs.py` & `p2pd-2.5.0/tests/test_net_afs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_p2p_pipe.py` & `p2pd-2.5.0/tests/test_p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_p2pd_server.py` & `p2pd-2.5.0/tests/test_p2pd_server.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_py_examples.py` & `p2pd-2.5.0/tests/test_py_examples.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_route.py` & `p2pd-2.5.0/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_route_table.py` & `p2pd-2.5.0/tests/test_route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_rudp.py` & `p2pd-2.5.0/tests/test_rudp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_signaling.py` & `p2pd-2.5.0/tests/test_signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_sock.py` & `p2pd-2.5.0/tests/test_sock.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,26 +25,29 @@
         s2.bind(('', port))
         #s2.connect(("www.google.com", 80))
 
         s1.close()
         s2.close()
 
     async def test_socket_factory_connect(self):
-        await init_p2pd()
-        loop = asyncio.get_event_loop()
-        i = await Interface().start_local()
+        loop = asyncio.get_running_loop()
+        netifaces = await init_p2pd()
+        i = await Interface(netifaces=netifaces).start_local()
         af = i.supported()[0]
-        r = await i.route(af).bind()
-        d = await Address("google.com", 80, r, TCP).res()
-        s = await socket_factory(r, dest_addr=d, sock_type=TCP)
-        await loop.sock_connect(
-            s, 
-            d.tup
+        r = await i.route(af).bind(0)
+        d = await Address("8.8.8.8", 53, r)
+        s = await socket_factory(route=r, dest_addr=d, sock_type=TCP, conf=NET_CONF)
+        con_task = asyncio.create_task(
+            loop.sock_connect(
+                s, 
+                d.tup
+            )
         )
 
+        await asyncio.wait_for(con_task, 2)
         if s is not None:
             s.close()
 
     async def test_high_port_reuse(self):
         # Config for reuse.
         conf = copy.deepcopy(NET_CONF)
         conf["reuse_addr"] = True
```

### Comparing `p2pd-2.4.1/tests/test_sorted_search.py` & `p2pd-2.5.0/tests/test_sorted_search.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_stun_client.py` & `p2pd-2.5.0/tests/test_stun_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             self.assertTrue(m[3]) # Mapped port
             IPRange(m[4]) # Is valid IP
 
             # Stun server addr.
             route = await i.route(af).bind()
             stun_server = STUNT_SERVERS[af][0]
             dest = await Address(
-                stun_server[0],
-                stun_server[1],
+                stun_server["primary"]["ip"],
+                stun_server["primary"]["port"],
                 route,
                 UDP
             ).res()
 
             # Check NAT test result is as expected.
             # Then check that other STUN requests work.
             if env.get("NAT_OPEN_INTERNET", False):
```

### Comparing `p2pd-2.4.1/tests/test_tcp_punch.py` & `p2pd-2.5.0/tests/test_tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_turn_client.py` & `p2pd-2.5.0/tests/test_turn_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.4.1/tests/test_win_netifaces.py` & `p2pd-2.5.0/tests/test_win_netifaces.py`

 * *Files identical despite different names*

