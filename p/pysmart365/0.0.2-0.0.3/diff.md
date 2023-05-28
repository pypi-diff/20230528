# Comparing `tmp/pysmart365-0.0.2.tar.gz` & `tmp/pysmart365-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.2.tar", last modified: Sun May 28 11:01:09 2023, max compression
+gzip compressed data, was "pysmart365-0.0.3.tar", last modified: Sun May 28 18:52:55 2023, max compression
```

## Comparing `pysmart365-0.0.2.tar` & `pysmart365-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:01:09.110862 pysmart365-0.0.2/
--rw-rw-rw-   0        0        0    35802 2023-05-27 14:51:46.000000 pysmart365-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      445 2023-05-28 11:01:09.100861 pysmart365-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-05-27 18:02:16.000000 pysmart365-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 11:01:09.065859 pysmart365-0.0.2/pysmart365/
--rw-rw-rw-   0        0        0      262 2023-05-28 10:59:09.000000 pysmart365-0.0.2/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     1745 2023-05-28 09:36:17.000000 pysmart365-0.0.2/pysmart365/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:01:09.089861 pysmart365-0.0.2/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      445 2023-05-28 11:01:08.000000 pysmart365-0.0.2/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-28 11:01:08.000000 pysmart365-0.0.2/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:01:08.000000 pysmart365-0.0.2/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 11:01:08.000000 pysmart365-0.0.2/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 11:01:09.112862 pysmart365-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-05-28 11:01:05.000000 pysmart365-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:52:55.765820 pysmart365-0.0.3/
+-rw-rw-rw-   0        0        0    35802 2023-05-27 14:51:46.000000 pysmart365-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      445 2023-05-28 18:52:55.763820 pysmart365-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-05-28 11:36:50.000000 pysmart365-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 18:52:55.726818 pysmart365-0.0.3/pysmart365/
+-rw-rw-rw-   0        0        0      475 2023-05-28 18:25:21.000000 pysmart365-0.0.3/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     2275 2023-05-28 18:19:39.000000 pysmart365-0.0.3/pysmart365/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:52:55.756820 pysmart365-0.0.3/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      445 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 18:52:55.767820 pysmart365-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-05-28 18:52:36.000000 pysmart365-0.0.3/setup.py
```

### Comparing `pysmart365-0.0.2/LICENSE` & `pysmart365-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.2/pysmart365/__init__.py` & `pysmart365-0.0.3/pysmart365/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 AUTHOR = 'Runkang'
 COPYRIGHT = '© Copyright 2023 Informatic365 - SmartSoft - MicroSoftware'
 
+class main():
+    print("Welcome to pysmart365 0.0.3")
+
 import subprocess
 import platform
 from customtkinter import *
 from tkinter import messagebox
 
 def turn_off(time):
     '''
@@ -43,8 +46,18 @@
         y = (shutdowngui.winfo_screenheight() - height) // 2
         shutdowngui.geometry(f"{width}x{height}+{x}+{y}")
         shutdowngui.title("Turn Off pc in gui mode")
         shutdown = CTkButton(shutdowngui, text="Turn Off", command=lambda: turn_off(time=0))
         shutdown.place(relx=0.5, rely=0.5, anchor='center')
         shutdowngui.mainloop()
     else:
-        subprocess.run(['slidetoshutdown'])
+        subprocess.run(['slidetoshutdown'])
+def copyright_view(year, company):
+    '''
+    Enter the copyright text that will be displayed with the name that you can customize and the year using the attribute 'company' for the name and 'year' for the year.
+    Example if i write copyright_view(year='2022 - 2023', company= 'Informatic365')
+    then displays "© Copyright 2022 - 2023 Informatic365".
+    '''
+    get = f'© Copyright {year} {company}'
+    return get
+if __name__ == '__main__':
+    main()
```

