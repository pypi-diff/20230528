# Comparing `tmp/wave_viewer-0.2.0.tar.gz` & `tmp/wave_viewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wave_viewer-0.2.0.tar", max compression
+gzip compressed data, was "wave_viewer-0.2.1.tar", max compression
```

## Comparing `wave_viewer-0.2.0.tar` & `wave_viewer-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-18 02:42:58.397916 wave_viewer-0.2.0/LICENSE
--rw-r--r--   0        0        0      837 2023-05-22 20:05:58.786520 wave_viewer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-05-18 02:38:54.638436 wave_viewer-0.2.0/README.md
--rw-r--r--   0        0        0      714 2023-05-22 20:04:53.097291 wave_viewer-0.2.0/wave_viewer/__init__.py
--rw-r--r--   0        0        0     4878 2023-05-22 20:04:53.098329 wave_viewer-0.2.0/wave_viewer/_controller.py
--rw-r--r--   0        0        0     6048 2023-05-22 20:04:53.099012 wave_viewer-0.2.0/wave_viewer/_viewer.py
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 wave_viewer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-18 02:42:58.397916 wave_viewer-0.2.1/LICENSE
+-rw-r--r--   0        0        0      837 2023-05-28 11:56:12.971870 wave_viewer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-05-28 11:53:04.265234 wave_viewer-0.2.1/README.md
+-rw-r--r--   0        0        0      714 2023-05-22 20:04:53.097291 wave_viewer-0.2.1/wave_viewer/__init__.py
+-rw-r--r--   0        0        0     5017 2023-05-28 11:42:11.245757 wave_viewer-0.2.1/wave_viewer/_controller.py
+-rw-r--r--   0        0        0     7110 2023-05-28 11:31:20.511591 wave_viewer-0.2.1/wave_viewer/_viewer.py
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 wave_viewer-0.2.1/PKG-INFO
```

### Comparing `wave_viewer-0.2.0/LICENSE` & `wave_viewer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.2.0/pyproject.toml` & `wave_viewer-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wave-viewer"
-version = "0.2.0"
+version = "0.2.1"
 description = "A simple GUI for viewing waveforms."
 authors = ["Jiahao Yuan <kaho0769@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kahojyun/wave-viewer"
 packages = [{include = "wave_viewer"}]
```

### Comparing `wave_viewer-0.2.0/wave_viewer/__init__.py` & `wave_viewer-0.2.1/wave_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.2.0/wave_viewer/_controller.py` & `wave_viewer-0.2.1/wave_viewer/_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,24 +24,24 @@
         process will be terminated when the main process exits. If False, the
         viewer process will continue to run after the main process exits. In this
         case, the viewer process must be closed manually by calling the `close`
         method. The default is True.
     """
 
     def __init__(self, daemon: bool = True) -> None:
-        self._rconn, self._wconn = mp.Pipe(duplex=False)
-        self._process = mp.Process(target=main, args=(self._rconn,), daemon=daemon)
+        self._conn = mp.Queue()
+        self._process = mp.Process(target=main, args=(self._conn,), daemon=daemon)
         self._process.start()
 
     def _ensure_open(self) -> None:
         if not self._process.is_alive():
             raise RuntimeError("WaveViewer is closed")
 
     def add_line(self, name: str, t: np.ndarray, ys: list, offset: float) -> None:
-        """Add a line to the plot.
+        """Add a line to the plot or update an existing line.
 
         The method accepts a list of y values and plots them against the time axis.
         The y values are plotted with different colors. The name will also be added
         to the right of the line.
 
         If a line with the same name already exists, it is replaced.
 
@@ -92,15 +92,15 @@
         msg = {
             "type": "add_line",
             "name": name,
             "t": t,
             "ys": ys,
             "offset": offset,
         }
-        self._wconn.send(msg)
+        self._conn.put(msg)
 
     def remove_line(self, name: str) -> None:
         """Remove a line from the plot.
 
         Parameters
         ----------
         name : str
@@ -113,43 +113,47 @@
         RuntimeError
             If the WaveViewer is closed.
         """
         self._ensure_open()
         if not isinstance(name, str):
             raise TypeError("name must be a string")
         msg = {"type": "remove_line", "name": name}
-        self._wconn.send(msg)
+        self._conn.put(msg)
 
     def clear(self) -> None:
         """Clear the plot.
 
+        Caution
+        -------
+        Lag may occur if the plot is cleared too frequently. You don't need to
+        clear the plot if you are updating the same lines.
+
         Raises
         ------
         RuntimeError
             If the WaveViewer is closed.
         """
         self._ensure_open()
         msg = {"type": "clear"}
-        self._wconn.send(msg)
+        self._conn.put(msg)
 
     def autoscale(self) -> None:
         """Autoscale the plot.
 
         Raises
         ------
         RuntimeError
             If the WaveViewer is closed.
         """
         self._ensure_open()
         msg = {"type": "autoscale"}
-        self._wconn.send(msg)
+        self._conn.put(msg)
 
     def close(self) -> None:
         """Close the WaveViewer."""
         self._process.terminate()
         self._process.join()
-        self._wconn.close()
-        self._rconn.close()
+        self._conn.close()
 
     def wait(self) -> None:
         """Wait for the WaveViewer to close."""
         self._process.join()
```

### Comparing `wave_viewer-0.2.0/PKG-INFO` & `wave_viewer-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wave-viewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple GUI for viewing waveforms.
 Home-page: https://github.com/kahojyun/wave-viewer
 License: MIT
 Author: Jiahao Yuan
 Author-email: kaho0769@qq.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -33,41 +33,48 @@
 
 ```bash
 pip install wave-viewer
 ```
 
 ## Usage
 
+Below is a simple example of how to use the `WaveViewer` class. Avoid calling
+`clear` if you only want to update the plot. It is more efficient to update the
+plot with `add_line`.
+
 ```python
 from wave_viewer import WaveViewer
 import numpy as np
 
-# Create the viewer
-viewer = WaveViewer()
 
-# Add a line to the plot
-x = np.arange(100000) / 2e9
-y = np.exp(1j * 2 * np.pi * 1e6 * x)
-ys = [y.real, y.imag]
-viewer.add_line("line1", x, ys, offset=0)
-
-# Add another line to the plot
-viewer.add_line("line2", x, ys, offset=2)
-
-# Auto scale the plot
-viewer.autoscale()
-
-# Remove the first line
-viewer.remove_line("line1")
-
-# Replace the second line
-y = np.exp(1j * 2 * np.pi * 2e6 * x)
-ys = [y.real, y.imag]
-viewer.add_line("line2", x, ys, offset=2)
+# This if statement is required for multiprocessing on Windows
+if __name__ == "__main__":
+    # Create the viewer
+    viewer = WaveViewer()
+
+    # Add a line to the plot
+    x = np.arange(100000) / 2e9
+    y = np.exp(1j * 2 * np.pi * 1e6 * x)
+    ys = [y.real, y.imag]
+    viewer.add_line("line1", x, ys, offset=0)
+
+    # Add another line to the plot
+    viewer.add_line("line2", x, ys, offset=2)
+
+    # Auto scale the plot
+    viewer.autoscale()
+
+    # Remove the first line
+    viewer.remove_line("line1")
+
+    # Replace the second line
+    y = np.exp(1j * 2 * np.pi * 2e6 * x)
+    ys = [y.real, y.imag]
+    viewer.add_line("line2", x, ys, offset=2)
 
-# Clear the plot
-viewer.clear()
+    # Clear the plot
+    viewer.clear()
 
-# Close the GUI
-viewer.close()
+    # Close the GUI
+    viewer.close()
 ```
```

