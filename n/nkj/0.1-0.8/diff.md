# Comparing `tmp/nkj-0.1.tar.gz` & `tmp/nkj-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkj-0.1.tar", last modified: Mon May 22 09:36:53 2023, max compression
+gzip compressed data, was "nkj-0.8.tar", last modified: Sun May 28 06:48:41 2023, max compression
```

## Comparing `nkj-0.1.tar` & `nkj-0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-05-22 09:36:53.141173 nkj-0.1/
--rw-r--r--   0 nakajima   (501) staff       (20)      150 2023-05-22 09:36:53.140481 nkj-0.1/PKG-INFO
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-05-22 09:36:53.134715 nkj-0.1/nkj/
--rw-r--r--   0 nakajima   (501) staff       (20)      190 2023-05-22 09:16:20.000000 nkj-0.1/nkj/__init__.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1760 2023-05-02 17:38:40.000000 nkj-0.1/nkj/arg.py
--rw-r--r--   0 nakajima   (501) staff       (20)    14061 2023-05-02 17:58:12.000000 nkj-0.1/nkj/cam.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1232 2023-05-03 06:08:21.000000 nkj-0.1/nkj/core.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3593 2023-05-02 18:05:13.000000 nkj-0.1/nkj/cv.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2322 2023-05-02 17:56:18.000000 nkj-0.1/nkj/ea.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2393 2023-05-02 17:46:49.000000 nkj-0.1/nkj/fa.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2325 2023-05-02 17:50:02.000000 nkj-0.1/nkj/file.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3857 2023-05-19 07:00:21.000000 nkj-0.1/nkj/filter.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1150 2023-05-02 17:34:25.000000 nkj-0.1/nkj/json.py
--rw-r--r--   0 nakajima   (501) staff       (20)    69960 2023-05-07 18:10:18.000000 nkj-0.1/nkj/math.py
--rw-r--r--   0 nakajima   (501) staff       (20)      502 2023-05-02 15:36:15.000000 nkj-0.1/nkj/np.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1638 2023-05-02 17:37:18.000000 nkj-0.1/nkj/os.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2149 2023-05-02 15:36:15.000000 nkj-0.1/nkj/plot.py
--rw-r--r--   0 nakajima   (501) staff       (20)      701 2023-05-02 17:17:27.000000 nkj-0.1/nkj/prob.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3326 2023-05-03 03:21:09.000000 nkj-0.1/nkj/pygame.py
--rw-r--r--   0 nakajima   (501) staff       (20)     9145 2023-05-03 03:23:05.000000 nkj-0.1/nkj/serial.py
--rw-r--r--   0 nakajima   (501) staff       (20)      186 2023-05-02 17:55:10.000000 nkj-0.1/nkj/socket.py
--rw-r--r--   0 nakajima   (501) staff       (20)     5356 2023-05-02 17:41:44.000000 nkj-0.1/nkj/stat.py
--rw-r--r--   0 nakajima   (501) staff       (20)     5572 2023-05-03 06:13:43.000000 nkj-0.1/nkj/str.py
--rw-r--r--   0 nakajima   (501) staff       (20)    21885 2023-05-19 07:00:21.000000 nkj-0.1/nkj/wavelet.py
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-05-22 09:36:53.139121 nkj-0.1/nkj.egg-info/
--rw-r--r--   0 nakajima   (501) staff       (20)      150 2023-05-22 09:36:53.000000 nkj-0.1/nkj.egg-info/PKG-INFO
--rw-r--r--   0 nakajima   (501) staff       (20)      370 2023-05-22 09:36:53.000000 nkj-0.1/nkj.egg-info/SOURCES.txt
--rw-r--r--   0 nakajima   (501) staff       (20)        1 2023-05-22 09:36:53.000000 nkj-0.1/nkj.egg-info/dependency_links.txt
--rw-r--r--   0 nakajima   (501) staff       (20)        4 2023-05-22 09:36:53.000000 nkj-0.1/nkj.egg-info/top_level.txt
--rw-r--r--   0 nakajima   (501) staff       (20)       38 2023-05-22 09:36:53.141394 nkj-0.1/setup.cfg
--rw-r--r--   0 nakajima   (501) staff       (20)      284 2023-05-22 09:12:42.000000 nkj-0.1/setup.py
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-05-28 06:48:41.955017 nkj-0.8/
+-rw-r--r--   0 nakajima   (501) staff       (20)      150 2023-05-28 06:48:41.954896 nkj-0.8/PKG-INFO
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-05-28 06:48:41.954143 nkj-0.8/nkj/
+-rw-r--r--   0 nakajima   (501) staff       (20)      190 2023-05-22 09:16:20.000000 nkj-0.8/nkj/__init__.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1760 2023-05-02 17:38:40.000000 nkj-0.8/nkj/arg.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    14061 2023-05-02 17:58:12.000000 nkj-0.8/nkj/cam.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1232 2023-05-03 06:08:21.000000 nkj-0.8/nkj/core.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3593 2023-05-02 18:05:13.000000 nkj-0.8/nkj/cv.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    22700 2023-05-28 06:46:17.000000 nkj-0.8/nkj/cwt.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2322 2023-05-02 17:56:18.000000 nkj-0.8/nkj/ea.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2393 2023-05-02 17:46:49.000000 nkj-0.8/nkj/fa.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2325 2023-05-02 17:50:02.000000 nkj-0.8/nkj/file.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3857 2023-05-19 07:00:21.000000 nkj-0.8/nkj/filter.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1150 2023-05-02 17:34:25.000000 nkj-0.8/nkj/json.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    69960 2023-05-07 18:10:18.000000 nkj-0.8/nkj/math.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      502 2023-05-02 15:36:15.000000 nkj-0.8/nkj/np.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1638 2023-05-02 17:37:18.000000 nkj-0.8/nkj/os.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2149 2023-05-02 15:36:15.000000 nkj-0.8/nkj/plot.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      701 2023-05-02 17:17:27.000000 nkj-0.8/nkj/prob.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3326 2023-05-03 03:21:09.000000 nkj-0.8/nkj/pygame.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     9145 2023-05-03 03:23:05.000000 nkj-0.8/nkj/serial.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      186 2023-05-02 17:55:10.000000 nkj-0.8/nkj/socket.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     5356 2023-05-02 17:41:44.000000 nkj-0.8/nkj/stat.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     5572 2023-05-03 06:13:43.000000 nkj-0.8/nkj/str.py
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-05-28 06:48:41.954738 nkj-0.8/nkj.egg-info/
+-rw-r--r--   0 nakajima   (501) staff       (20)      150 2023-05-28 06:48:41.000000 nkj-0.8/nkj.egg-info/PKG-INFO
+-rw-r--r--   0 nakajima   (501) staff       (20)      366 2023-05-28 06:48:41.000000 nkj-0.8/nkj.egg-info/SOURCES.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)        1 2023-05-28 06:48:41.000000 nkj-0.8/nkj.egg-info/dependency_links.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)        4 2023-05-28 06:48:41.000000 nkj-0.8/nkj.egg-info/top_level.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)       38 2023-05-28 06:48:41.955059 nkj-0.8/setup.cfg
+-rw-r--r--   0 nakajima   (501) staff       (20)      284 2023-05-28 06:46:59.000000 nkj-0.8/setup.py
```

### Comparing `nkj-0.1/nkj/arg.py` & `nkj-0.8/nkj/arg.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/cam.py` & `nkj-0.8/nkj/cam.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/core.py` & `nkj-0.8/nkj/core.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/cv.py` & `nkj-0.8/nkj/cv.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/ea.py` & `nkj-0.8/nkj/ea.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/fa.py` & `nkj-0.8/nkj/fa.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/file.py` & `nkj-0.8/nkj/file.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/filter.py` & `nkj-0.8/nkj/filter.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/json.py` & `nkj-0.8/nkj/json.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/math.py` & `nkj-0.8/nkj/math.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/os.py` & `nkj-0.8/nkj/os.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/plot.py` & `nkj-0.8/nkj/plot.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/prob.py` & `nkj-0.8/nkj/prob.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/pygame.py` & `nkj-0.8/nkj/pygame.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/serial.py` & `nkj-0.8/nkj/serial.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/stat.py` & `nkj-0.8/nkj/stat.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/str.py` & `nkj-0.8/nkj/str.py`

 * *Files identical despite different names*

### Comparing `nkj-0.1/nkj/wavelet.py` & `nkj-0.8/nkj/cwt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
-# [name] nkj.wavelet.py
-# [exec] python -m nkj.wavelet
+# [name] nkj.cwt.py
+# [exec] python -m nkj.cwt
 #
 # Written by Yoshikazu NAKAJIMA
 #
 _LIB_DEBUGLEVEL = 0
 
 import os
 import sys
@@ -143,19 +143,88 @@
 def morlet_wt(wt): # wt: angle [-np.pi, np.pi]
 	gx = wavelet_gauss_time(wt / (2.0 * np.pi))
 	g = exp(-sq(gx) / 2.0) # gauss
 	re = g * cos(wt)
 	im = g * sin(wt)
 	return re, im
 
+def normalize_kernel(kernel_re, kernel_im):
+	__VERSION = 2
+
+	if (__VERSION == 1):
+		# bias elimination
+
+		dmean = mean([mean(kernel_re), mean(kernel_im)])
+		kernel_re -= dmean
+		kernel_im -= dmean
+
+		dsum = 0.0
+		for i in range(len(kernel_re)):
+			dsum += sqrt(sq(kernel_re[i]) + sq(kernel_im[i]))
+		dsum /= 2.0 # due to dividing to real and imaginary
+
+		if (dsum != 0.0):
+			kernel_re /= dsum
+			kernel_im /= dsum
+
+	elif (__VERSION == 2):
+		#
+		# kernel の re, im それぞれに対して、さらに +, - 成分をそれぞれで算出し、各々の重み和が 0.5 になるように補正する．
+		#
+		rpsum = 0.0  # real positive
+		rnsum = 0.0  # real negative
+		ipsum = 0.0  # imaginary positive
+		insum = 0.0  # imaginary negative
+
+		for i in range(len(kernel_re)):
+			re = kernel_re[i]
+			if (re >= 0.0):
+				rpsum += re
+			else:
+				rnsum -= re   # += -re
+
+		for j in range(len(kernel_im)):
+			im = kernel_im[j]
+			if (im >= 0.0):
+				ipsum += im
+			else:
+				insum -= im   # += -im
+
+		rpsum *= 2.0   # /= 0.5
+		rnsum *= 2.0   # /= 0.5
+		ipsum *= 2.0   # /= 0.5
+		insum *= 2.0   # /= 0.5
+
+		for i in range(len(kernel_re)):
+			if (kernel_re[i] >= 0.0):
+				if (rpsum != 0.0):
+					kernel_re[i] /= rpsum
+			else:
+				if (rnsum != 0.0):
+					kernel_re[i] /= rnsum
+
+		for j in range(len(kernel_im)):
+			if (kernel_im[j] >= 0.0):
+				if (ipsum != 0.0):
+					kernel_im[j] /= ipsum
+			else:
+				if (insum != 0.0):
+					kernel_im[j] /= insum
+
+	else: # other versions
+		kernel_re = gain_normalization(bias_elimination(kernel_re))
+		kernel_im = gain_normalization(bias_elimination(kernel_im))
+
+	return kernel_re, kernel_im
+
 def morlet_kernel(f, dt):
-	"""
-	f:  Analyzed frequency [Hz]
-	dt: Sampling interval(time/length)
-	"""
+	#
+	# f:  Analyzed frequency [Hz]
+	# dt: Sampling interval(time/length)
+	#
 	ldprint2(["Analized frequency: ", f])
 
 	fs = 1.0 / dt
 	ldprint2(["Sampling frequency: ", fs])
 
 	if (fs < 2.0 * f):
 		print_error("Too low sampling frequency.")
@@ -188,85 +257,31 @@
 		elif (_WAVELET_FUNCTION == "morlet"):
 			re, im = morlet(t, f)
 		else:
 			print_error("Illegal _WAVELET_FUNCTION specification.")
 			os.sys.exit()
 		kernel_re.append(re)
 		kernel_im.append(im)
+
 	kernel_re = np.array(kernel_re)
 	kernel_im = np.array(kernel_im)
 
-	# bias elimination
-
-	dmean = mean([mean(kernel_re), mean(kernel_im)])
-	kernel_re -= dmean
-	kernel_im -= dmean
-
 	# kernel normalization
 
-	# version 1
-	"""
-	dsum = 0.0
-	for i in range(len(kernel_re)):
-		dsum += sqrt(sq(kernel_re[i]) + sq(kernel_im[i]))
-	dsum /= 2.0 # due to dividing to real and imaginary
-
-	if (dsum != 0.0):
-		kernel_re /= dsum
-		kernel_im /= dsum
-	"""
-
-	# version 2
-	rpsum = 0.0
-	rnsum = 0.0
-	ipsum = 0.0
-	insum = 0.0
-	for i in range(len(kernel_re)):
-		re = kernel_re[i]
-		im = kernel_im[i]
-		if (re >= 0.0):
-			rpsum += re
-		else:
-			rnsum += re
-		if (im >= 0.0):
-			ipsum += im
-		else:
-			insum += im
-
-	rpsum /= 0.5
-	rnsum /= 0.5
-	ipsum /= 0.5
-	insum /= 0.5
-
-	for i in range(len(kernel_re)):
-		if (kernel_re[i] >= 0.0):
-			kernel_re[i] = (rpsum == 0.0) ? kernel_re[i] : (kernel_re[i] / rpsum)
-		else:
-			kernel_re[i] = (rnsum == 0.0) ? kernel_re[i] : (kernel_re[i] / rnsum)
-
-		if (kernel_im[i] >= 0.0):
-			kernel_im[i] = (ipsum == 0.0) ? kernel_im[i] : (kernel_im[i] / ipsum)
-		else:
-			kernel_im[i] = (insum == 0.0) ? kernel_im[i] : (kernel_im[i] / insum)
-
-	"""
-	# other versions
-	kernel_re = gain_normalization(bias_elimination(kernel_re))
-	kernel_im = gain_normalization(bias_elimination(kernel_im))
-	"""
+	kernel_re, kernel_im = normalize_kernel(kernel_re, kernel_im)
 
 	return kernel_re, kernel_im, kernelsize
 
-def wavelet_f(data, dt, f): # dt: sampling interval, f: analyzed frequency
+def wavelet_f(data, dt, f): # dt: sampling interval [sec], f: analyzed frequency [Hz]
 	ldprint2(["--> wavelet_f(data[", len(data), "], ", dt, ", ", f, ")"])
 
 	datasize = len(data)
 	ldprint2(["Data size: ", datasize])
 
-	kr, ki, ks = morlet_kernel(f, dt)
+	kr, ki, ks = morlet_kernel(f, dt)  # 周波数とサンプリング間隔（秒）からカーネルを生成
 	ldprint2(["Filter size: ", ks])
 
 	footsize = foot_size(ks)
 	ldprint2(["Foot size:   ", footsize])
 
 	offset = kernel_offset(ks)
 	ldprint2(["Offset:      ", offset])
@@ -292,19 +307,19 @@
 		ldprint2(["Kernel size: ", ks])
 		if (len(signal) != ks):
 			'''
 			print_error("Too short data compared with the analyzed frequency of {0:0.3f} Hz. Wavelet cycle length exceeded over the data size. Data are padded with {1:0.3f}.".format(f, error_padding()))
 			'''
 			dlen = len(data)
 			return False, np.full(dlen, error_padding(), dtype=np.float), np.full(dlen, error_padding(), dtype=np.float), np.full(dlen, error_padding(), dtype=np.float)
-		re = np.dot(signal, kr)
-		im = np.dot(signal, ki)
-		wt.append(sqrt(sq(re) + sq(im)))
-		wt_im.append(re)
-		wt_re.append(im)
+		re = np.dot(signal, kr)   # 信号とカーネルの内積をとる
+		im = np.dot(signal, ki)   # 信号とカーネルの内積をとる
+		wt.append(sqrt(sq(re) + sq(im)))   # 実部と虚部からパワーを計算
+		wt_re.append(re)
+		wt_im.append(im)
 		index += 1
 		if (data_bias_elimination_flag()):
 			del signal
 			gc.collect()
 
 	while (index < datasize - offset):
 		left = index - offset
@@ -313,16 +328,16 @@
 		if (data_bias_elimination_flag()):
 			signal = bias_elimination(data[left : right])
 		else:
 			signal = data[left : right]
 		re = np.dot(signal, kr)
 		im = np.dot(signal, ki)
 		wt.append(sqrt(sq(re) + sq(im)))
-		wt_im.append(re)
-		wt_re.append(im)
+		wt_re.append(re)
+		wt_im.append(im)
 		index += 1
 		if (data_bias_elimination_flag()):
 			del signal
 			gc.collect()
 
 	while (index < datasize):
 		left = index - offset
@@ -336,25 +351,28 @@
 		if (data_bias_elimination_flag()):
 			signal = bias_elimination(np.array(concatenate([ldata, rdata])))
 		else:
 			signal = np.array(concatenate([ldata, rdata]))
 		re = np.dot(signal, kr)
 		im = np.dot(signal, ki)
 		wt.append(sqrt(sq(re) + sq(im)))
-		wt_im.append(re)
-		wt_re.append(im)
+		wt_re.append(re)
+		wt_im.append(im)
 		index += 1
 		if (data_bias_elimination_flag()):
 			del signal
 			gc.collect()
 
 	ldprint2(["<-- wavelet_f()"])
 
 	return True, np.array(wt), np.array(wt_re), np.array(wt_im)
 
+def cwt_f(data, dt, f):
+	return wavelet_f(data, dt, f)
+
 def wavelet(data, dt, flist): # flist: frequency list
 	ldprint(["--> wavelet(data[", len(data), "], ", dt, ")"])
 	slist = []
 	warray = np.empty((0, len(data)))
 	rarray = np.empty((0, len(data)))
 	iarray = np.empty((0, len(data)))
 	for f in flist:
@@ -367,14 +385,17 @@
 		slist.append(status)
 		warray = np.vstack((warray, wt))
 		rarray = np.vstack((rarray, wt_re))
 		iarray = np.vstack((iarray, wt_im))
 	ldprint(["<-- wavelet()"])
 	return slist, warray, rarray, iarray
 
+def cwt(data, dt, flist):
+	return wavelet(data, dt, flist)
+
 def power_normalize_ws(data): # data: wavelet spectra
 	ldprint(["--> power_normalize_ws()"])
 	ldprint(["Data shape: ", data.shape])
 
 	freqs = data.shape[0]
 	samples = data.shape[1]
 	ldprint(["Frequencies:  ", freqs])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

