# Comparing `tmp/hidapi-0.9.0.post2.tar.gz` & `tmp/hidapi-0.9.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hidapi-0.9.0.post2.tar", last modified: Fri Feb  7 22:56:00 2020, max compression
+gzip compressed data, was "dist/hidapi-0.9.0.post3.tar", last modified: Sat Jun 20 09:04:09 2020, max compression
```

## Comparing `hidapi-0.9.0.post2.tar` & `hidapi-0.9.0.post3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/
--rw-r--r--   0 stick     (1000) users      (100)     1517 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/LICENSE-bsd.txt
--rw-r--r--   0 stick     (1000) users      (100)    35147 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/LICENSE-gpl3.txt
--rw-r--r--   0 stick     (1000) users      (100)       87 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/LICENSE-orig.txt
--rw-r--r--   0 stick     (1000) users      (100)      558 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/LICENSE.txt
--rw-r--r--   0 stick     (1000) users      (100)      193 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/MANIFEST.in
--rw-r--r--   0 stick     (1000) users      (100)     1014 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/PKG-INFO
--rw-r--r--   0 stick     (1000) users      (100)     2094 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/README.rst
--rw-r--r--   0 stick     (1000) users      (100)     1437 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/chid.pxd
--rw-r--r--   0 stick     (1000) users      (100)     6461 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/hid.pyx
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi/
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi/hidapi/
--rw-r--r--   0 stick     (1000) users      (100)    15760 2020-02-03 19:36:41.000000 hidapi-0.9.0.post2/hidapi/hidapi/hidapi.h
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi/libusb/
--rw-r--r--   0 stick     (1000) users      (100)    42005 2020-02-03 19:36:41.000000 hidapi-0.9.0.post2/hidapi/libusb/hid.c
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi/linux/
--rw-r--r--   0 stick     (1000) users      (100)    21727 2020-02-03 19:36:41.000000 hidapi-0.9.0.post2/hidapi/linux/hid.c
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi/mac/
--rw-r--r--   0 stick     (1000) users      (100)    33689 2020-02-03 19:36:41.000000 hidapi-0.9.0.post2/hidapi/mac/hid.c
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi/windows/
--rwxr-xr-x   0 stick     (1000) users      (100)    27746 2020-02-03 19:36:41.000000 hidapi-0.9.0.post2/hidapi/windows/hid.c
-drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi.egg-info/
--rw-r--r--   0 stick     (1000) users      (100)     1014 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi.egg-info/PKG-INFO
--rw-r--r--   0 stick     (1000) users      (100)      386 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi.egg-info/SOURCES.txt
--rw-r--r--   0 stick     (1000) users      (100)        1 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi.egg-info/dependency_links.txt
--rw-r--r--   0 stick     (1000) users      (100)       17 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi.egg-info/requires.txt
--rw-r--r--   0 stick     (1000) users      (100)       11 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/hidapi.egg-info/top_level.txt
--rw-r--r--   0 stick     (1000) users      (100)     6461 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/hidraw.pyx
--rw-r--r--   0 stick     (1000) users      (100)       38 2020-02-07 22:56:00.000000 hidapi-0.9.0.post2/setup.cfg
--rwxr-xr-x   0 stick     (1000) users      (100)     4199 2020-02-07 22:32:40.000000 hidapi-0.9.0.post2/setup.py
--rw-r--r--   0 stick     (1000) users      (100)      195 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/tests.py
--rw-r--r--   0 stick     (1000) users      (100)     1200 2019-08-10 16:57:54.000000 hidapi-0.9.0.post2/try.py
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.752252 hidapi-0.9.0.post3/
+-rw-r--r--   0 stick     (1000) users      (100)     1517 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/LICENSE-bsd.txt
+-rw-r--r--   0 stick     (1000) users      (100)    35147 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/LICENSE-gpl3.txt
+-rw-r--r--   0 stick     (1000) users      (100)       87 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/LICENSE-orig.txt
+-rw-r--r--   0 stick     (1000) users      (100)      558 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/LICENSE.txt
+-rw-r--r--   0 stick     (1000) users      (100)      193 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/MANIFEST.in
+-rw-r--r--   0 stick     (1000) users      (100)      818 2020-06-20 09:04:09.752252 hidapi-0.9.0.post3/PKG-INFO
+-rw-r--r--   0 stick     (1000) users      (100)     2094 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/README.rst
+-rw-r--r--   0 stick     (1000) users      (100)     1572 2020-06-20 08:52:34.000000 hidapi-0.9.0.post3/chid.pxd
+-rw-r--r--   0 stick     (1000) users      (100)     7485 2020-06-20 08:52:34.000000 hidapi-0.9.0.post3/hid.pyx
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.746253 hidapi-0.9.0.post3/hidapi/
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.750253 hidapi-0.9.0.post3/hidapi/hidapi/
+-rw-r--r--   0 stick     (1000) users      (100)    15760 2020-02-03 19:36:41.000000 hidapi-0.9.0.post3/hidapi/hidapi/hidapi.h
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.751252 hidapi-0.9.0.post3/hidapi/libusb/
+-rw-r--r--   0 stick     (1000) users      (100)    42123 2020-06-20 08:55:46.000000 hidapi-0.9.0.post3/hidapi/libusb/hid.c
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.751252 hidapi-0.9.0.post3/hidapi/linux/
+-rw-r--r--   0 stick     (1000) users      (100)    21727 2020-02-03 19:36:41.000000 hidapi-0.9.0.post3/hidapi/linux/hid.c
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.751252 hidapi-0.9.0.post3/hidapi/mac/
+-rw-r--r--   0 stick     (1000) users      (100)    33697 2020-06-20 08:55:46.000000 hidapi-0.9.0.post3/hidapi/mac/hid.c
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.752252 hidapi-0.9.0.post3/hidapi/windows/
+-rwxr-xr-x   0 stick     (1000) users      (100)    27741 2020-06-20 08:55:46.000000 hidapi-0.9.0.post3/hidapi/windows/hid.c
+drwxr-xr-x   0 stick     (1000) users      (100)        0 2020-06-20 09:04:09.750253 hidapi-0.9.0.post3/hidapi.egg-info/
+-rw-r--r--   0 stick     (1000) users      (100)      818 2020-06-20 09:04:09.000000 hidapi-0.9.0.post3/hidapi.egg-info/PKG-INFO
+-rw-r--r--   0 stick     (1000) users      (100)      386 2020-06-20 09:04:09.000000 hidapi-0.9.0.post3/hidapi.egg-info/SOURCES.txt
+-rw-r--r--   0 stick     (1000) users      (100)        1 2020-06-20 09:04:09.000000 hidapi-0.9.0.post3/hidapi.egg-info/dependency_links.txt
+-rw-r--r--   0 stick     (1000) users      (100)       17 2020-06-20 09:04:09.000000 hidapi-0.9.0.post3/hidapi.egg-info/requires.txt
+-rw-r--r--   0 stick     (1000) users      (100)       11 2020-06-20 09:04:09.000000 hidapi-0.9.0.post3/hidapi.egg-info/top_level.txt
+-rw-r--r--   0 stick     (1000) users      (100)     7485 2020-06-20 08:52:34.000000 hidapi-0.9.0.post3/hidraw.pyx
+-rw-r--r--   0 stick     (1000) users      (100)       38 2020-06-20 09:04:09.752252 hidapi-0.9.0.post3/setup.cfg
+-rwxr-xr-x   0 stick     (1000) users      (100)     4007 2020-06-20 08:56:50.000000 hidapi-0.9.0.post3/setup.py
+-rw-r--r--   0 stick     (1000) users      (100)      195 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/tests.py
+-rw-r--r--   0 stick     (1000) users      (100)     1200 2019-08-10 16:57:54.000000 hidapi-0.9.0.post3/try.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hidapi-0.9.0.post2/LICENSE-bsd.txt` & `hidapi-0.9.0.post3/LICENSE-bsd.txt`

 * *Files identical despite different names*

### Comparing `hidapi-0.9.0.post2/LICENSE-gpl3.txt` & `hidapi-0.9.0.post3/LICENSE-gpl3.txt`

 * *Files identical despite different names*

### Comparing `hidapi-0.9.0.post2/LICENSE.txt` & `hidapi-0.9.0.post3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hidapi-0.9.0.post2/PKG-INFO` & `hidapi-0.9.0.post3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 1.2
 Name: hidapi
-Version: 0.9.0.post2
+Version: 0.9.0.post3
 Summary: A Cython interface to the hidapi from https://github.com/libusb/hidapi
 Home-page: https://github.com/trezor/cython-hidapi
 Author: Gary Bishop
 Author-email: gb@cs.unc.edu
 Maintainer: Pavol Rusnak
 Maintainer-email: pavol@rusnak.io
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hidapi-0.9.0.post2/README.rst` & `hidapi-0.9.0.post3/README.rst`

 * *Files identical despite different names*

### Comparing `hidapi-0.9.0.post2/chid.pxd` & `hidapi-0.9.0.post3/chid.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     unsigned short usage_page
     unsigned short usage
     int interface_number
     hid_device_info *next
 
   hid_device_info* hid_enumerate(unsigned short, unsigned short)
   void hid_free_enumeration(hid_device_info*)
-  int hid_exit()
 
   hid_device* hid_open(unsigned short, unsigned short, const wchar_t*)
   hid_device* hid_open_path(char *path)
   void hid_close(hid_device *)
   int hid_write(hid_device* device, unsigned char *data, int length) nogil
   int hid_read(hid_device* device, unsigned char* data, int max_length) nogil
   int hid_read_timeout(hid_device* device, unsigned char* data, int max_length, int milliseconds) nogil
   int hid_set_nonblocking(hid_device* device, int value)
   int hid_send_feature_report(hid_device* device, unsigned char *data, int length) nogil
   int hid_get_feature_report(hid_device* device, unsigned char *data, int length) nogil
+  int hid_get_input_report(hid_device* device, unsigned char *data, int length) nogil
 
   int hid_get_manufacturer_string(hid_device*, wchar_t *, size_t)
   int hid_get_product_string(hid_device*, wchar_t *, size_t)
   int hid_get_serial_number_string(hid_device*, wchar_t *, size_t)
+  int hid_get_indexed_string(hid_device*, int, wchar_t *, size_t)
   wchar_t *hid_error(hid_device *)
```

### Comparing `hidapi-0.9.0.post2/hid.pyx` & `hidapi-0.9.0.post3/hid.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -71,15 +71,14 @@
       if self._c_hid == NULL:
           raise IOError('open failed')
 
   def close(self):
       if self._c_hid != NULL:
           hid_close(self._c_hid)
           self._c_hid = NULL
-          hid_exit()
 
   def write(self, buff):
       '''Accept a list of integers (0-255) and send them to the device'''
       if self._c_hid == NULL:
           raise ValueError('not open')
       # convert to bytes
       if sys.version_info < (3, 0):
@@ -152,14 +151,24 @@
           raise ValueError('not open')
       cdef wchar_t buff[255]
       cdef int r = hid_get_serial_number_string(self._c_hid, buff, 255)
       if r < 0:
           raise IOError('get serial number string error')
       return U(buff)
 
+  def get_indexed_string(self, index):
+    if self._c_hid == NULL:
+      raise ValueError('not open')
+    cdef wchar_t buff[255]
+    cdef unsigned char c_index = index
+    cdef int r = hid_get_indexed_string(self._c_hid, c_index, buff, 255)
+    if r < 0:
+        raise IOError('get indexed string error')
+    return U(buff)
+
   def send_feature_report(self, buff):
       if self._c_hid == NULL:
           raise ValueError('not open')
       '''Accept a list of integers (0-255) and send them to the device'''
       # convert to bytes
       if sys.version_info < (3, 0):
           buff = ''.join(map(chr, buff))
@@ -191,13 +200,37 @@
       res = []
       if n < 0:
           raise IOError('read error')
       for i in range(n):
           res.append(cbuff[i])
       if max_length > 16:
           free(cbuff)
+      return res
+
+  def get_input_report(self, int report_num, int max_length):
+      if self._c_hid == NULL:
+          raise ValueError('not open')
+      cdef hid_device * c_hid = self._c_hid
+      cdef unsigned char lbuff[16]
+      cdef unsigned char* cbuff
+      cdef size_t c_max_length = max_length
+      cdef int n
+      if max_length <= 16:
+          cbuff = lbuff
+      else:
+          cbuff = <unsigned char *>malloc(max_length)
+      cbuff[0] = report_num
+      with nogil:
+          n = hid_get_input_report(c_hid, cbuff, c_max_length)
+      res = []
+      if n < 0:
+          raise IOError('read error')
+      for i in range(n):
+          res.append(cbuff[i])
+      if max_length > 16:
+          free(cbuff)
       return res
 
   def error(self):
       if self._c_hid == NULL:
           raise ValueError('not open')
       return U(<wchar_t*>hid_error(self._c_hid))
```

### Comparing `hidapi-0.9.0.post2/hidapi/hidapi/hidapi.h` & `hidapi-0.9.0.post3/hidapi/hidapi/hidapi.h`

 * *Files identical despite different names*

### Comparing `hidapi-0.9.0.post2/hidapi/libusb/hid.c` & `hidapi-0.9.0.post3/hidapi/libusb/hid.c`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 #include <sys/utsname.h>
 #include <fcntl.h>
 #include <pthread.h>
 #include <wchar.h>
 
 /* GNU / LibUSB */
 #include <libusb.h>
-#ifndef __ANDROID__
+#if !defined(__ANDROID__) && !defined(NO_ICONV)
 #include <iconv.h>
 #endif
 
 #include "hidapi.h"
 
 #if defined(__ANDROID__) && __ANDROID_API__ < __ANDROID_API_N__
 
@@ -391,15 +391,15 @@
    by using free(). */
 static wchar_t *get_usb_string(libusb_device_handle *dev, uint8_t idx)
 {
 	char buf[512];
 	int len;
 	wchar_t *str = NULL;
 
-#ifndef __ANDROID__ /* we don't use iconv on Android */
+#if !defined(__ANDROID__) && !defined(NO_ICONV) /* we don't use iconv on Android, or when it is explicitly disabled */
 	wchar_t wbuf[256];
 	/* iconv variables */
 	iconv_t ic;
 	size_t inbytes;
 	size_t outbytes;
 	size_t res;
 	char *inptr;
@@ -417,15 +417,15 @@
 			idx,
 			lang,
 			(unsigned char*)buf,
 			sizeof(buf));
 	if (len < 0)
 		return NULL;
 
-#ifdef __ANDROID__
+#if defined(__ANDROID__) || defined(NO_ICONV)
 
 	/* Bionic does not have iconv support nor wcsdup() function, so it
 	   has to be done manually.  The following code will only work for
 	   code points that can be represented as a single UTF-16 character,
 	   and will incorrectly convert any code points which require more
 	   than one UTF-16 character.
```

### Comparing `hidapi-0.9.0.post2/hidapi/linux/hid.c` & `hidapi-0.9.0.post3/hidapi/linux/hid.c`

 * *Files identical despite different names*

### Comparing `hidapi-0.9.0.post2/hidapi/mac/hid.c` & `hidapi-0.9.0.post3/hidapi/mac/hid.c`

 * *Files 1% similar despite different names*

```diff
@@ -823,15 +823,15 @@
 
 		/* Create the buffers for receiving data */
 		dev->max_input_report_len = (CFIndex) get_max_report_length(dev->device_handle);
 		dev->input_report_buf = (uint8_t*) calloc(dev->max_input_report_len, sizeof(uint8_t));
 
 		/* Create the Run Loop Mode for this device.
 		   printing the reference seems to work. */
-		sprintf(str, "HIDAPI_%p", dev->device_handle);
+		sprintf(str, "HIDAPI_%p", (void*) dev->device_handle);
 		dev->run_loop_mode =
 			CFStringCreateWithCString(NULL, str, kCFStringEncodingASCII);
 
 		/* Attach the device to a Run Loop */
 		IOHIDDeviceRegisterInputReportCallback(
 			dev->device_handle, dev->input_report_buf, dev->max_input_report_len,
 			&hid_report_callback, dev);
```

### Comparing `hidapi-0.9.0.post2/hidapi/windows/hid.c` & `hidapi-0.9.0.post3/hidapi/windows/hid.c`

 * *Files 0% similar despite different names*

```diff
@@ -824,29 +824,29 @@
 	return bytes_returned;
 #endif
 }
 
 
 int HID_API_EXPORT HID_API_CALL hid_get_input_report(hid_device *dev, unsigned char *data, size_t length)
 {
-#if 0
 	BOOL res;
+#if 0
 	res = HidD_GetInputReport(dev->device_handle, data, length);
 	if (!res) {
 		register_error(dev, "HidD_GetInputReport");
 		return -1;
 	}
 	return length;
 #else
 	DWORD bytes_returned;
 
 	OVERLAPPED ol;
 	memset(&ol, 0, sizeof(ol));
 
-	BOOL res = DeviceIoControl(dev->device_handle,
+	res = DeviceIoControl(dev->device_handle,
 		IOCTL_HID_GET_INPUT_REPORT,
 		data, length,
 		data, length,
 		&bytes_returned, &ol);
 
 	if (!res) {
 		if (GetLastError() != ERROR_IO_PENDING) {
```

### Comparing `hidapi-0.9.0.post2/hidapi.egg-info/PKG-INFO` & `hidapi-0.9.0.post3/hidapi.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 1.2
 Name: hidapi
-Version: 0.9.0.post2
+Version: 0.9.0.post3
 Summary: A Cython interface to the hidapi from https://github.com/libusb/hidapi
 Home-page: https://github.com/trezor/cython-hidapi
 Author: Gary Bishop
 Author-email: gb@cs.unc.edu
 Maintainer: Pavol Rusnak
 Maintainer-email: pavol@rusnak.io
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hidapi-0.9.0.post2/hidraw.pyx` & `hidapi-0.9.0.post3/hidraw.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -71,15 +71,14 @@
       if self._c_hid == NULL:
           raise IOError('open failed')
 
   def close(self):
       if self._c_hid != NULL:
           hid_close(self._c_hid)
           self._c_hid = NULL
-          hid_exit()
 
   def write(self, buff):
       '''Accept a list of integers (0-255) and send them to the device'''
       if self._c_hid == NULL:
           raise ValueError('not open')
       # convert to bytes
       if sys.version_info < (3, 0):
@@ -152,14 +151,24 @@
           raise ValueError('not open')
       cdef wchar_t buff[255]
       cdef int r = hid_get_serial_number_string(self._c_hid, buff, 255)
       if r < 0:
           raise IOError('get serial number string error')
       return U(buff)
 
+  def get_indexed_string(self, index):
+    if self._c_hid == NULL:
+      raise ValueError('not open')
+    cdef wchar_t buff[255]
+    cdef unsigned char c_index = index
+    cdef int r = hid_get_indexed_string(self._c_hid, c_index, buff, 255)
+    if r < 0:
+        raise IOError('get indexed string error')
+    return U(buff)
+
   def send_feature_report(self, buff):
       if self._c_hid == NULL:
           raise ValueError('not open')
       '''Accept a list of integers (0-255) and send them to the device'''
       # convert to bytes
       if sys.version_info < (3, 0):
           buff = ''.join(map(chr, buff))
@@ -191,13 +200,37 @@
       res = []
       if n < 0:
           raise IOError('read error')
       for i in range(n):
           res.append(cbuff[i])
       if max_length > 16:
           free(cbuff)
+      return res
+
+  def get_input_report(self, int report_num, int max_length):
+      if self._c_hid == NULL:
+          raise ValueError('not open')
+      cdef hid_device * c_hid = self._c_hid
+      cdef unsigned char lbuff[16]
+      cdef unsigned char* cbuff
+      cdef size_t c_max_length = max_length
+      cdef int n
+      if max_length <= 16:
+          cbuff = lbuff
+      else:
+          cbuff = <unsigned char *>malloc(max_length)
+      cbuff[0] = report_num
+      with nogil:
+          n = hid_get_input_report(c_hid, cbuff, c_max_length)
+      res = []
+      if n < 0:
+          raise IOError('read error')
+      for i in range(n):
+          res.append(cbuff[i])
+      if max_length > 16:
+          free(cbuff)
       return res
 
   def error(self):
       if self._c_hid == NULL:
           raise ValueError('not open')
       return U(<wchar_t*>hid_error(self._c_hid))
```

### Comparing `hidapi-0.9.0.post2/setup.py` & `hidapi-0.9.0.post3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -101,34 +101,30 @@
             include_dirs = include_dirs_bsd,
             libraries = libs,
             )
         ]
 
 setup(
     name = 'hidapi',
-    version = '0.9.0.post2',
+    version = '0.9.0.post3',
     description = 'A Cython interface to the hidapi from https://github.com/libusb/hidapi',
     author = 'Gary Bishop',
     author_email = 'gb@cs.unc.edu',
     maintainer = 'Pavol Rusnak',
     maintainer_email = 'pavol@rusnak.io',
     url = 'https://github.com/trezor/cython-hidapi',
     package_dir = {'hid': 'hidapi/*'},
     classifiers = [
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'License :: OSI Approved :: BSD License',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
     ],
     ext_modules = modules,
     setup_requires = ['Cython'],
     install_requires = ['setuptools>=19.0'],
 )
```

### Comparing `hidapi-0.9.0.post2/try.py` & `hidapi-0.9.0.post3/try.py`

 * *Files identical despite different names*

