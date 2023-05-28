# Comparing `tmp/ipyeos-0.4.0.tar.gz` & `tmp/ipyeos-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyeos-0.4.0.tar", last modified: Sat May 27 13:00:02 2023, max compression
+gzip compressed data, was "ipyeos-0.4.1.tar", last modified: Sun May 28 02:30:42 2023, max compression
```

## Comparing `ipyeos-0.4.0.tar` & `ipyeos-0.4.1.tar`

### file list

```diff
@@ -1,118 +1,38 @@
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.711957 ipyeos-0.4.0/
--rw-r--r--   0 newworld   (502) staff       (20)     1063 2022-09-05 23:06:37.000000 ipyeos-0.4.0/LICENSE
--rw-r--r--   0 newworld   (502) staff       (20)      174 2022-09-05 23:06:37.000000 ipyeos-0.4.0/MANIFEST.in
--rw-r--r--   0 newworld   (502) staff       (20)     3466 2023-05-27 13:00:02.712226 ipyeos-0.4.0/PKG-INFO
--rw-r--r--   0 newworld   (502) staff       (20)     3272 2023-05-22 04:32:55.000000 ipyeos-0.4.0/README.md
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.919989 ipyeos-0.4.0/_skbuild/
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.920127 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.934300 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/
--rw-r--r--   0 newworld   (502) staff       (20)     1063 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/LICENSE
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.958589 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/
--rw-r--r--   0 newworld   (502) staff       (20)     1395 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/__init__.py
--rw-r--r--   0 newworld   (502) staff       (20)     2140 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/__main__.py
--rwxr-xr-x   0 newworld   (502) staff       (20)   523560 2023-05-21 13:24:24.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/_eos.cpython-310-darwin.so
--rw-r--r--   0 newworld   (502) staff       (20)    17367 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/chain.py
--rw-r--r--   0 newworld   (502) staff       (20)    16936 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/chainapi.py
--rw-r--r--   0 newworld   (502) staff       (20)    30998 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/chaintester.py
--rw-r--r--   0 newworld   (502) staff       (20)    10424 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/config.py
--rw-r--r--   0 newworld   (502) staff       (20)     3433 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/eos.py
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.983485 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/
--rw-r--r--   0 newworld   (502) staff       (20)   877453 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/Apply.py
--rw-r--r--   0 newworld   (502) staff       (20)    15889 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/ApplyRequest.py
--rw-r--r--   0 newworld   (502) staff       (20)   156885 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/IPCChainTester.py
--rw-r--r--   0 newworld   (502) staff       (20)     8156 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/PushActions.py
--rw-r--r--   0 newworld   (502) staff       (20)       92 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/__init__.py
--rw-r--r--   0 newworld   (502) staff       (20)      366 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/constants.py
--rw-r--r--   0 newworld   (502) staff       (20)    31953 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/ttypes.py
--rw-r--r--   0 newworld   (502) staff       (20)      204 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/log.py
--rw-r--r--   0 newworld   (502) staff       (20)      238 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/main.py
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.920951 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/release/
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.994605 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/release/bin/
--rwxr-xr-x   0 newworld   (502) staff       (20) 35702144 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/release/bin/ipyeos
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.459066 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/release/lib/
--rwxr-xr-x   0 newworld   (502) staff       (20)    16608 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/release/lib/libchain_api.dylib
--rwxr-xr-x   0 newworld   (502) staff       (20)    40336 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/release/lib/libvm_api.dylib
--rw-r--r--   0 newworld   (502) staff       (20)     5426 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/rpc_server.py
--rw-r--r--   0 newworld   (502) staff       (20)     2687 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/run.py
--rw-r--r--   0 newworld   (502) staff       (20)    52216 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/server.py
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.467255 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/
--rw-r--r--   0 newworld   (502) staff       (20)      610 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/activate_kv.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.922538 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.475075 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.bios/
--rw-r--r--   0 newworld   (502) staff       (20)    20720 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.bios/eosio.bios.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)    18589 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.bios/eosio.bios.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.487964 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.msig/
--rw-r--r--   0 newworld   (502) staff       (20)    12047 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.msig/eosio.msig.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)    28553 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.msig/eosio.msig.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.502908 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.system/
--rw-r--r--   0 newworld   (502) staff       (20)    75982 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.system/eosio.system.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)   383975 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.system/eosio.system.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.520325 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.token/
--rw-r--r--   0 newworld   (502) staff       (20)     8577 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.token/eosio.token.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)    17637 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.token/eosio.token.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.524896 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.wrap/
--rw-r--r--   0 newworld   (502) staff       (20)     3754 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.wrap/eosio.wrap.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)     2088 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/eosio.wrap/eosio.wrap.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.543530 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/micropython/
--rw-r--r--   0 newworld   (502) staff       (20)     6078 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/micropython/micropython.abi
--rw-r--r--   0 newworld   (502) staff       (20)   266852 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/micropython/micropython.wasm
--rw-r--r--   0 newworld   (502) staff       (20)   273560 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/contracts/micropython/micropython_eosio.wasm
--rw-r--r--   0 newworld   (502) staff       (20)      815 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/tests/test_template.py
--rw-r--r--   0 newworld   (502) staff       (20)       27 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/types.py
--rw-r--r--   0 newworld   (502) staff       (20)       27 2023-05-21 13:47:19.000000 ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/requirements.txt
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.553674 ipyeos-0.4.0/ipyeos.egg-info/
--rw-r--r--   0 newworld   (502) staff       (20)     3466 2023-05-27 13:00:01.000000 ipyeos-0.4.0/ipyeos.egg-info/PKG-INFO
--rw-r--r--   0 newworld   (502) staff       (20)     4654 2023-05-27 13:00:01.000000 ipyeos-0.4.0/ipyeos.egg-info/SOURCES.txt
--rw-r--r--   0 newworld   (502) staff       (20)        1 2023-05-27 13:00:01.000000 ipyeos-0.4.0/ipyeos.egg-info/dependency_links.txt
--rw-r--r--   0 newworld   (502) staff       (20)      114 2023-05-27 13:00:01.000000 ipyeos-0.4.0/ipyeos.egg-info/entry_points.txt
--rw-r--r--   0 newworld   (502) staff       (20)       58 2023-05-27 13:00:01.000000 ipyeos-0.4.0/ipyeos.egg-info/requires.txt
--rw-r--r--   0 newworld   (502) staff       (20)        7 2023-05-27 13:00:01.000000 ipyeos-0.4.0/ipyeos.egg-info/top_level.txt
--rw-r--r--   0 newworld   (502) staff       (20)       84 2022-09-05 23:06:37.000000 ipyeos-0.4.0/pyproject.toml
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.593469 ipyeos-0.4.0/pysrc/
--rw-r--r--   0 newworld   (502) staff       (20)     1394 2023-05-22 04:33:31.000000 ipyeos-0.4.0/pysrc/__init__.py
--rw-r--r--   0 newworld   (502) staff       (20)     2140 2023-05-21 04:26:38.000000 ipyeos-0.4.0/pysrc/__main__.py
--rw-r--r--   0 newworld   (502) staff       (20)    17367 2023-01-10 15:48:40.000000 ipyeos-0.4.0/pysrc/chain.py
--rw-r--r--   0 newworld   (502) staff       (20)    16936 2023-05-15 07:11:18.000000 ipyeos-0.4.0/pysrc/chainapi.py
--rw-r--r--   0 newworld   (502) staff       (20)    31105 2023-05-25 02:14:17.000000 ipyeos-0.4.0/pysrc/chaintester.py
--rw-r--r--   0 newworld   (502) staff       (20)    10424 2022-09-05 23:06:37.000000 ipyeos-0.4.0/pysrc/config.py
--rw-r--r--   0 newworld   (502) staff       (20)     3433 2023-05-21 13:15:39.000000 ipyeos-0.4.0/pysrc/eos.py
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.634184 ipyeos-0.4.0/pysrc/interfaces/
--rw-r--r--   0 newworld   (502) staff       (20)   877453 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/Apply.py
--rw-r--r--   0 newworld   (502) staff       (20)    15889 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/ApplyRequest.py
--rw-r--r--   0 newworld   (502) staff       (20)   156885 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/IPCChainTester.py
--rw-r--r--   0 newworld   (502) staff       (20)     8156 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/PushActions.py
--rw-r--r--   0 newworld   (502) staff       (20)       92 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/__init__.py
--rw-r--r--   0 newworld   (502) staff       (20)      366 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/constants.py
--rw-r--r--   0 newworld   (502) staff       (20)    31953 2022-10-28 13:26:00.000000 ipyeos-0.4.0/pysrc/interfaces/ttypes.py
--rw-r--r--   0 newworld   (502) staff       (20)      204 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/log.py
--rw-r--r--   0 newworld   (502) staff       (20)      238 2022-11-01 08:40:36.000000 ipyeos-0.4.0/pysrc/main.py
--rw-r--r--   0 newworld   (502) staff       (20)     5426 2023-02-11 14:30:54.000000 ipyeos-0.4.0/pysrc/rpc_server.py
--rw-r--r--   0 newworld   (502) staff       (20)     2692 2023-05-22 04:21:58.000000 ipyeos-0.4.0/pysrc/run.py
--rw-r--r--   0 newworld   (502) staff       (20)    52216 2023-02-11 14:31:49.000000 ipyeos-0.4.0/pysrc/server.py
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.640007 ipyeos-0.4.0/pysrc/tests/
--rw-r--r--   0 newworld   (502) staff       (20)      610 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/activate_kv.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:01.925483 ipyeos-0.4.0/pysrc/tests/contracts/
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.642795 ipyeos-0.4.0/pysrc/tests/contracts/eosio.bios/
--rw-r--r--   0 newworld   (502) staff       (20)    20720 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.bios/eosio.bios.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)    18589 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.bios/eosio.bios.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.648497 ipyeos-0.4.0/pysrc/tests/contracts/eosio.msig/
--rw-r--r--   0 newworld   (502) staff       (20)    12047 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.msig/eosio.msig.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)    28553 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.msig/eosio.msig.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.653654 ipyeos-0.4.0/pysrc/tests/contracts/eosio.system/
--rw-r--r--   0 newworld   (502) staff       (20)    75982 2022-09-09 02:47:13.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.system/eosio.system.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)   383975 2022-09-09 02:47:13.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.system/eosio.system.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.673726 ipyeos-0.4.0/pysrc/tests/contracts/eosio.token/
--rw-r--r--   0 newworld   (502) staff       (20)     8577 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.token/eosio.token.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)    17637 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.token/eosio.token.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.687312 ipyeos-0.4.0/pysrc/tests/contracts/eosio.wrap/
--rw-r--r--   0 newworld   (502) staff       (20)     3754 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.wrap/eosio.wrap.abi
--rwxr-xr-x   0 newworld   (502) staff       (20)     2088 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/eosio.wrap/eosio.wrap.wasm
-drwxr-xr-x   0 newworld   (502) staff       (20)        0 2023-05-27 13:00:02.700513 ipyeos-0.4.0/pysrc/tests/contracts/micropython/
--rw-r--r--   0 newworld   (502) staff       (20)     6078 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/micropython/micropython.abi
--rw-r--r--   0 newworld   (502) staff       (20)   266852 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/micropython/micropython.wasm
--rw-r--r--   0 newworld   (502) staff       (20)   273560 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/contracts/micropython/micropython_eosio.wasm
--rw-r--r--   0 newworld   (502) staff       (20)      815 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/tests/test_template.py
--rw-r--r--   0 newworld   (502) staff       (20)       27 2022-09-05 23:06:38.000000 ipyeos-0.4.0/pysrc/types.py
--rw-r--r--   0 newworld   (502) staff       (20)       27 2022-09-05 23:06:38.000000 ipyeos-0.4.0/requirements.txt
--rw-r--r--   0 newworld   (502) staff       (20)      272 2023-05-27 13:00:02.713724 ipyeos-0.4.0/setup.cfg
--rw-r--r--   0 newworld   (502) staff       (20)     1270 2023-05-22 04:32:58.000000 ipyeos-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.631235 ipyeos-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-28 02:30:35.000000 ipyeos-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-28 02:30:35.000000 ipyeos-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-05-28 02:30:42.631235 ipyeos-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-05-28 02:30:35.000000 ipyeos-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.627235 ipyeos-0.4.1/ipyeos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.627235 ipyeos-0.4.1/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17367 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16936 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/chainapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31105 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/chaintester.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.631235 ipyeos-0.4.1/pysrc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/Apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/ApplyRequest.py
+-rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/IPCChainTester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/PushActions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52216 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-28 02:30:35.000000 ipyeos-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-28 02:30:42.631235 ipyeos-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-05-28 02:30:35.000000 ipyeos-0.4.1/setup.py
```

### Comparing `ipyeos-0.4.0/LICENSE` & `ipyeos-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/PKG-INFO` & `ipyeos-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.0
+Version: 0.4.1
 Summary: IPYEOS project
+Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Interactive Python for Eos
@@ -57,15 +58,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.0**.whl
+python3 -m pip install dist/pyeos-0.4.1**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.0/README.md` & `ipyeos-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.0**.whl
+python3 -m pip install dist/pyeos-0.4.1**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/__init__.py` & `ipyeos-0.4.1/pysrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shlex
 import platform
 import subprocess
 import sysconfig
 import argparse
 from . import run
 
-__version__ = "0.3.11"
+__version__ = "0.4.1"
 
 class CustomImporter(object):
     def find_module(self, fullname, mpath=None):
 #        print('+++find_module', fullname)
         if fullname in ['_chain', '_chainapi', '_vm_api']:
             return self
         return
```

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/__main__.py` & `ipyeos-0.4.1/pysrc/__main__.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/chain.py` & `ipyeos-0.4.1/pysrc/chain.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/chainapi.py` & `ipyeos-0.4.1/pysrc/chainapi.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/chaintester.py` & `ipyeos-0.4.1/pysrc/chaintester.py`

 * *Files 3% similar despite different names*

```diff
@@ -712,29 +712,29 @@
                 self.code_cache[src] = code
                 return code
         except Exception as e:
             raise e
         finally:
             os.chdir(cur_dir)
 
-    def get_balance(self, account):
+    def get_balance(self, account, token_account: str='eosio.token', symbol: str='EOS'):
         try:
             ret = self.api.get_table_rows(
                 True,
-                'eosio.token',
+                token_account,
                 account,
                 'accounts',
-                '',
-                '',
+                symbol,
+                symbol,
                 10
             )
             balance = ret['rows'][0]['balance'].split(' ')[0]
-            return round(float(balance) * 10000) / 10000
+            return int(balance.replace('.', ''))
         except Exception as e:
-            logger.info(e)
+            logger.exception(e)
             return 0.0
 
     def get_table_rows(self, _json, code, scope, table,
                                     lower_bound, upper_bound,
                                     limit,
                                     key_type='',
                                     index_position='', 
@@ -744,18 +744,18 @@
         key_type: "i64"|"i128"|"i256"|"float64"|"float128"|"sha256"|"ripemd160"
         index_position: "2"|"3"|"4"|"5"|"6"|"7"|"8"|"9"|"10"
         """
         return self.api.get_table_rows(
             _json, code, scope, table,
             lower_bound, upper_bound,
             limit,
-            '',
-            '', 
-            reverse,
-            show_payer            
+            key_type=key_type,
+            index_position=index_position, 
+            reverse=reverse,
+            show_payer=show_payer
         )
 
     def s2n(self, s: str) -> int:
         return eos.s2n(s)
 
     def n2s(self, n: int) -> str:
         return eos.n2s(n)
```

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/config.py` & `ipyeos-0.4.1/pysrc/config.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/eos.py` & `ipyeos-0.4.1/pysrc/eos.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/Apply.py` & `ipyeos-0.4.1/pysrc/interfaces/Apply.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/ApplyRequest.py` & `ipyeos-0.4.1/pysrc/interfaces/ApplyRequest.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/IPCChainTester.py` & `ipyeos-0.4.1/pysrc/interfaces/IPCChainTester.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/PushActions.py` & `ipyeos-0.4.1/pysrc/interfaces/PushActions.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/interfaces/ttypes.py` & `ipyeos-0.4.1/pysrc/interfaces/ttypes.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/rpc_server.py` & `ipyeos-0.4.1/pysrc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/run.py` & `ipyeos-0.4.1/pysrc/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 
 def run_ipyeos(custom_cmds=None):
     if 'RUN_IPYEOS' in os.environ:
         print('ipyeos command can only be called by python')
         return
 
     if platform.system() == 'Windows' or is_macos_arm():
-        cmd = f'docker run --entrypoint ipyeos -it -v "{os.getcwd()}:/develop" -w /develop -t ghcr.io/uuosio/ipyeos'
+        cmd = f'docker run --entrypoint ipyeos -it --rm -v "{os.getcwd()}:/develop" -w /develop -t ghcr.io/uuosio/ipyeos'
         cmd = shlex.split(cmd)
-        cmd.extend(sys.argv[1:])
+        if not custom_cmds:
+            cmd.extend(sys.argv[1:])
+        else:
+            cmd.extend(custom_cmds)
         print(' '.join(cmd))
         return subprocess.call(cmd, stdout=sys.stdout, stderr=sys.stderr)
 
     dir_name = os.path.dirname(os.path.realpath(__file__))
     dir_name = os.path.join(dir_name, "release")
     ipyeos_program = os.path.join(dir_name, "bin/ipyeos")
 
@@ -55,16 +58,16 @@
     return subprocess.call(cmds, stdout=sys.stdout, stderr=sys.stderr)
 
 def run_eosnode(custom_cmds=None):
     run_ipyeos(custom_cmds)
 
 def start_debug_server():
     if platform.system() == 'Windows':
-        cmd = f'docker run --rm -it -w /root/dev -v "{os.getcwd()}:/root/dev" -t gscdk/test'
+        cmd = f'docker run --rm -it -w /root/dev -v "{os.getcwd()}:/root/dev" -p 9090:9090 -p 9092:9092 -p 9093:9093 -t ghcr.io/uuosio/ipyeos'
         cmd = shlex.split(cmd)
-        cmd.append(sys.argv[1:])
+        cmd.extend(sys.argv[1:])
         print(' '.join(cmd))
         return subprocess.call(cmd, stdout=sys.stdout, stderr=sys.stderr)
 
     custom_cmds = ['-m', 'ipyeos', 'eosdebugger']
     custom_cmds.extend(sys.argv[1:])
     run_ipyeos(custom_cmds)
```

### Comparing `ipyeos-0.4.0/_skbuild/macosx-10.15-x86_64-3.10/cmake-install/pysrc/server.py` & `ipyeos-0.4.1/pysrc/server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.0/ipyeos.egg-info/PKG-INFO` & `ipyeos-0.4.1/ipyeos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.0
+Version: 0.4.1
 Summary: IPYEOS project
+Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Interactive Python for Eos
@@ -57,15 +58,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.0**.whl
+python3 -m pip install dist/pyeos-0.4.1**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.0/setup.py` & `ipyeos-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'tests/contracts/micropython/*',
     'tests/test_template.py',
     'tests/activate_kv.wasm',
 ])
 
 setup(
     name="ipyeos",
-    version="0.4.0",
+    version="0.4.1",
     description="IPYEOS project",
     author='The IPYEOS Team',
     license="MIT",
     packages=[
         'ipyeos',
         'ipyeos.interfaces'
     ],
```

