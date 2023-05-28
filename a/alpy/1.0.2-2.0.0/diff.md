# Comparing `tmp/alpy-1.0.2.tar.gz` & `tmp/alpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpy-1.0.2.tar", last modified: Tue May  3 10:07:38 2022, max compression
+gzip compressed data, was "alpy-2.0.0.tar", last modified: Sun May 28 13:44:42 2023, max compression
```

## Comparing `alpy-1.0.2.tar` & `alpy-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 10:07:38.441293 alpy-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-05-03 10:07:36.000000 alpy-1.0.2/COPYING
--rw-r--r--   0 root         (0) root         (0)    15475 2022-05-03 10:07:38.441293 alpy-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14412 2022-05-03 10:07:36.000000 alpy-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 10:07:38.439293 alpy-1.0.2/alpy/
--rw-rw-rw-   0 root         (0) root         (0)       89 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6167 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/console.py
--rw-rw-rw-   0 root         (0) root         (0)     9103 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/container.py
--rw-rw-rw-   0 root         (0) root         (0)    11169 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/node.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/pexpect_log.py
--rw-rw-rw-   0 root         (0) root         (0)     9299 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/qemu.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/remote_shell.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/run.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2022-05-03 10:07:36.000000 alpy-1.0.2/alpy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-03 10:07:38.441293 alpy-1.0.2/alpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15475 2022-05-03 10:07:38.000000 alpy-1.0.2/alpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2022-05-03 10:07:38.000000 alpy-1.0.2/alpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-03 10:07:38.000000 alpy-1.0.2/alpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-05-03 10:07:38.000000 alpy-1.0.2/alpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-05-03 10:07:38.000000 alpy-1.0.2/alpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-03 10:07:38.441293 alpy-1.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1335 2022-05-03 10:07:36.000000 alpy-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 13:44:42.864233 alpy-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-28 13:44:41.000000 alpy-2.0.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)    15489 2023-05-28 13:44:42.864233 alpy-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14412 2023-05-28 13:44:41.000000 alpy-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 13:44:42.863233 alpy-2.0.0/alpy/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     9103 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/container.py
+-rw-rw-rw-   0 root         (0) root         (0)    11164 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/pexpect_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     9508 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/qemu.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/remote_shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 13:44:42.864233 alpy-2.0.0/alpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15489 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 13:44:42.864233 alpy-2.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1385 2023-05-28 13:44:41.000000 alpy-2.0.0/setup.py
```

### Comparing `alpy-1.0.2/COPYING` & `alpy-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/PKG-INFO` & `alpy-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: alpy
-Version: 1.0.2
+Version: 2.0.0
 Summary: Library for testing network virtual appliances using Docker
 Home-page: https://gitlab.com/abogdanenko/alpy
 Author: Alexey Bogdanenko
 Author-email: alexey@bogdanenko.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 ####
@@ -436,9 +435,7 @@
 - `Virtual Networks over linuX (VNX)
   <http://web.dit.upm.es/vnxwiki/index.php/Main_Page>`_
 
 - `Pipework: Software-Defined Networking for Linux Containers
   <https://github.com/jpetazzo/pipework>`_
 
 - `Eve-NG <https://www.eve-ng.net/>`_
-
-
```

### Comparing `alpy-1.0.2/README.rst` & `alpy-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/alpy/console.py` & `alpy-2.0.0/alpy/console.py`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/alpy/container.py` & `alpy-2.0.0/alpy/container.py`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/alpy/node.py` & `alpy-2.0.0/alpy/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,53 +84,48 @@
         try:
             container.start()
             alpy.container.close(container, self._timeout)
         finally:
             container.remove()
 
     def _create_interface(self):
-
         self._run_in_container(
             self._iproute2_image,
             ["ip", "tuntap", "add", "mode", "tap", "dev", self._interface_name],
             network_mode="host",
             cap_add=["NET_ADMIN"],
             devices=["/dev/net/tun"],
         )
 
     def _move_interface_to_node_container(self):
-
         self._run_in_container(
             self._iproute2_image,
             ["ip", "link", "set", "netns", "1", "dev", self._interface_name],
             network_mode="host",
             pid_mode=self._join_node_ns,
             cap_add=["NET_ADMIN"],
         )
 
     def _rename_interface(self):
-
         self._run_in_container(
             self._busybox_image,
             ["ip", "link", "set", "name", "eth0", "dev", self._interface_name],
             network_mode=self._join_node_ns,
             cap_add=["NET_ADMIN"],
         )
 
     def _raise_interface(self):
-
         self._run_in_container(
             self._busybox_image,
             ["ip", "link", "set", "up", "dev", "eth0"],
             network_mode=self._join_node_ns,
             cap_add=["NET_ADMIN"],
         )
 
     def _remove_interface(self):
-
         self._run_in_container(
             self._busybox_image,
             ["ip", "link", "delete", "dev", self._interface_name],
             network_mode="host",
             cap_add=["NET_ADMIN"],
         )
```

### Comparing `alpy-1.0.2/alpy/pexpect_log.py` & `alpy-2.0.0/alpy/pexpect_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,17 +98,17 @@
     assigned to the :py:attr:`pexpect:pexpect.spawn.logfile_read` attribute.
 
     :param logger: logger
     :type logger: :py:class:`python:logging.Logger`
     """
 
     def __init__(self, logger):
-        log_function = lambda line: logger.debug(
-            "< " + format_bytes_for_logging(line)
-        )
+        def log_function(line):
+            logger.debug("< " + format_bytes_for_logging(line))
+
         self._splitter = Splitter(
             sep=b"\n", chunk_ready_callback=log_function, low=20, high=120
         )
 
     def write(self, data):
         """Accumulate data and write it to the log.
```

### Comparing `alpy-1.0.2/alpy/qemu.py` & `alpy-2.0.0/alpy/qemu.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,16 +228,26 @@
     :param tcp_port: TCP port to listen on
     :type tcp_port: int
     :return: list of arguments
     :rtype: list(str)
     """
     return [
         "-chardev",
-        f"socket,id=id_char_serial,port={tcp_port},"
-        "host=127.0.0.1,ipv4,nodelay,server,nowait,telnet,logfile=console.log",
+        (
+            "socket,"
+            "id=id_char_serial,"
+            f"port={tcp_port},"
+            "host=127.0.0.1,"
+            "ipv4=on,"
+            "nodelay=on,"
+            "server=on,"
+            "wait=off,"
+            "telnet=on,"
+            "logfile=console.log"
+        ),
         "-serial",
         "chardev:id_char_serial",
     ]
 
 
 @contextlib.contextmanager
 def temporary_copy_ovmf_vars():
@@ -282,15 +292,19 @@
     :rtype: list(str)
     """
     args = []
 
     # firmware executable code
     args.append("-drive")
     args.append(
-        "if=pflash,format=raw,unit=0,readonly,file=/usr/share/OVMF/OVMF_CODE.fd"
+        "if=pflash,"
+        "format=raw,"
+        "unit=0,"
+        "readonly=on,"
+        "file=/usr/share/OVMF/OVMF_CODE.fd"
     )
 
     # firmware variable store
     args.append("-drive")
     args.append("if=pflash,format=raw,unit=1,file=" + OVMF_VARS_COPY_FILENAME)
 
     return args
```

### Comparing `alpy-1.0.2/alpy/remote_shell.py` & `alpy-2.0.0/alpy/remote_shell.py`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/alpy/run.py` & `alpy-2.0.0/alpy/run.py`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/alpy/utils.py` & `alpy-2.0.0/alpy/utils.py`

 * *Files identical despite different names*

### Comparing `alpy-1.0.2/alpy.egg-info/PKG-INFO` & `alpy-2.0.0/alpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: alpy
-Version: 1.0.2
+Version: 2.0.0
 Summary: Library for testing network virtual appliances using Docker
 Home-page: https://gitlab.com/abogdanenko/alpy
 Author: Alexey Bogdanenko
 Author-email: alexey@bogdanenko.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 ####
@@ -436,9 +435,7 @@
 - `Virtual Networks over linuX (VNX)
   <http://web.dit.upm.es/vnxwiki/index.php/Main_Page>`_
 
 - `Pipework: Software-Defined Networking for Linux Containers
   <https://github.com/jpetazzo/pipework>`_
 
 - `Eve-NG <https://www.eve-ng.net/>`_
-
-
```

### Comparing `alpy-1.0.2/setup.py` & `alpy-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,12 +26,13 @@
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
     ],
 )
```

