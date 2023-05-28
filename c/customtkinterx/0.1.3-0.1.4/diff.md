# Comparing `tmp/customtkinterx-0.1.3.tar.gz` & `tmp/customtkinterx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.1.3.tar", max compression
+gzip compressed data, was "customtkinterx-0.1.4.tar", max compression
```

## Comparing `customtkinterx-0.1.3.tar` & `customtkinterx-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.3/customtkinterx/__init__.py
--rw-r--r--   0        0        0      175 2023-05-27 12:34:54.450444 customtkinterx-0.1.3/customtkinterx/__main__.py
--rw-r--r--   0        0        0     3776 2023-05-27 10:59:38.605996 customtkinterx-0.1.3/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     5306 2023-05-27 08:36:14.109297 customtkinterx-0.1.3/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     1204 2023-05-27 11:45:12.773768 customtkinterx-0.1.3/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     4688 2023-05-27 12:34:54.453461 customtkinterx-0.1.3/customtkinterx/Fluent.json
--rw-r--r--   0        0        0     2417 2023-05-27 12:33:24.813013 customtkinterx-0.1.3/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0      343 2023-05-27 12:35:25.385298 customtkinterx-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.3/README.md
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 customtkinterx-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.4/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      175 2023-05-27 12:34:54.450444 customtkinterx-0.1.4/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     4283 2023-05-28 11:12:48.677370 customtkinterx-0.1.4/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     5311 2023-05-27 14:55:38.518710 customtkinterx-0.1.4/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     1204 2023-05-27 11:45:12.773768 customtkinterx-0.1.4/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     4700 2023-05-27 15:00:01.395429 customtkinterx-0.1.4/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0     2417 2023-05-27 12:33:24.813013 customtkinterx-0.1.4/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0      343 2023-05-28 11:12:48.665370 customtkinterx-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.4/README.md
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 customtkinterx-0.1.4/PKG-INFO
```

### Comparing `customtkinterx-0.1.3/customtkinterx/CTkCustom.py` & `customtkinterx-0.1.4/customtkinterx/CTkCustom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-from customtkinter import CTk, CTkFrame, CTkLabel, CTkButton, ThemeManager, get_appearance_mode
+from customtkinter import CTk, CTkToplevel, CTkFrame, CTkLabel, CTkButton, ThemeManager, get_appearance_mode
 from tkinter import ttk
 from sys import platform
 
 
 class CTkCustom(CTk):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, title: str = "", advanced: bool = True, **kwargs):
+        try:
+            super().__init__(**kwargs)
+        except:
+            pass
         from customtkinterx import CTkFluentThemePath
-        if platform == "win32":
-            self.configure(fg_color="#101010")
-            self.wm_attributes("-transparentcolor", "#101010")
+        if advanced:
+            if platform == "win32":
+                self.configure(fg_color="#101010")
+                self.wm_attributes("-transparentcolor", "#101010")
 
         self.wm_overrideredirect(True)
 
-        try:
-            from ctypes import windll
-            GWL_EXSTYLE = -20
-            WS_EX_APPWINDOW = 0x00040000
-            WS_EX_TOOLWINDOW = 0x00000080
-            hwnd = windll.user32.GetParent(self.winfo_id())
-            style = windll.user32.GetWindowLongW(hwnd, GWL_EXSTYLE)
-            style = style & ~WS_EX_TOOLWINDOW
-            style = style | WS_EX_APPWINDOW
-            res = windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
-        except:
-            self.wm_attributes("-topmost", True)
+        if advanced:
+            if platform == "win32":
+                from ctypes import windll
+                GWL_EXSTYLE = -20
+                WS_EX_APPWINDOW = 0x00040000
+                WS_EX_TOOLWINDOW = 0x00000080
+                hwnd = windll.user32.GetParent(self.winfo_id())
+                style = windll.user32.GetWindowLongW(hwnd, GWL_EXSTYLE)
+                style = style & ~WS_EX_TOOLWINDOW
+                style = style | WS_EX_APPWINDOW
+                res = windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
+            else:
+                try:
+                    self.wm_attributes("-topmost", True)
+                except:
+                    pass
 
         self.minsize(150, 180)
 
         self.__frame_border = CTkFrame(self, border_width=1)
         self.__frame_border.pack(fill="both", expand=True, padx=0, pady=0)
 
         self.__frame_title = CTkFrame(self.__frame_border, border_width=0, corner_radius=2)
         self.__frame_title.pack(fill="x", side="top", padx=2, pady=2)
         self.bind_move(self.__frame_title)
 
-        self.__label_title = CTkLabel(self.__frame_title, text=self.wm_title())
+        self.__label_title = CTkLabel(self.__frame_title, text=title)
         self.__label_title.pack(side="left", anchor="w", padx=10, pady=5)
         self.bind_move(self.__label_title)
 
+        self.title(title)
+
         self.maximized = False
 
-        self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30, command=lambda: self.destroy())
+        self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30,
+                                        command=lambda: self.destroy())
         self.__button_close.pack(side="right", anchor="e", padx=5, pady=5)
 
-        self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30, command=lambda: self.minimize())
+        self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30,
+                                           command=lambda: self.minimize())
         self.__button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
 
         self.x, self.y = 0, 0
 
     def minimize(self):
         try:
             from ctypes import windll
@@ -94,12 +106,19 @@
         new_y = (event.y - self.y) + self.winfo_y()
         if new_y <= 0:
             new_y = 0
         s = f"+{new_x}+{new_y}"
         self.geometry(s)
 
 
+class CTkCustomToplevel(CTkCustom, CTkToplevel):
+    pass
+
+
 if __name__ == '__main__':
     root = CTkCustom()
     root.title("helloworld")
     root.titlebar_title.configure(text="helloworld")
-    root.mainloop()
+
+    CTkCustomToplevel(root)
+
+    root.mainloop()
```

### Comparing `customtkinterx-0.1.3/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.1.4/customtkinterx/CTkFluentTheme.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,20 @@
     "hover_color": ["#3B8ED0", "#1F6AA5"],
     "checkmark_color": ["#DCE4EE", "gray90"],
     "text_color": ["gray10", "#DCE4EE"],
     "text_color_disabled": ["gray60", "gray45"]
   },
   "CTkSwitch": {
     "corner_radius": 1000,
-    "border_width": 0,
+    "border_width": 1,
     "button_length": 0,
     "fg_color": ["#939BA2", "#4A4D50"],
     "progress_color": ["#0067c0", "#4cc2ff"],
-    "button_color": ["gray36", "#D5D9DE"],
-    "button_hover_color": ["gray20", "gray100"],
+    "button_color": ["#f3f3f3", "#000000"],
+    "button_hover_color": ["#bfbfbf", "#050505"],
     "text_color": ["gray10", "#DCE4EE"],
     "text_color_disabled": ["gray60", "gray45"]
   },
   "CTkRadiobutton": {
     "corner_radius": 1000,
     "border_width_checked": 6,
     "border_width_unchecked": 3,
@@ -128,17 +128,17 @@
     "scrollbar_button_color": ["gray55", "gray41"],
     "scrollbar_button_hover_color": ["gray40", "gray53"]
   },
   "CTkScrollableFrame": {
     "label_fg_color": ["gray78", "gray23"]
   },
   "DropdownMenu": {
-    "fg_color": ["gray90", "gray20"],
-    "hover_color": ["gray75", "gray28"],
-    "text_color": ["gray10", "gray90"]
+    "fg_color": ["gray90", "#1c1c1c"],
+    "hover_color": ["gray75", "#313131"],
+    "text_color": ["gray10", "#ffffff"]
   },
   "CTkFont": {
     "macOS": {
       "family": "SF Display",
       "size": 13,
       "weight": "normal"
     },
```

### Comparing `customtkinterx-0.1.3/customtkinterx/CTkListBox.py` & `customtkinterx-0.1.4/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.3/customtkinterx/Fluent.json` & `customtkinterx-0.1.4/customtkinterx/Fluent.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631577%*

 * *Differences: {"'CTkFont'": "{'Windows': {'family': 'Microsoft YaHei', 'size': 12}}",*

 * * "'CTkSwitch'": "{'border_width': 0.1, 'fg_color': ['#ededed', '#1d1d1d']}",*

 * * "'DropdownMenu'": "{'fg_color': {insert: [(1, '#1c1c1c')], delete: [1]}, 'hover_color': {insert: "*

 * *                   "[(1, '#313131')], delete: [1]}, 'text_color': {insert: [(1, '#ffffff')], "*

 * *                   'delete: [1]}}'}*

```diff
@@ -108,16 +108,16 @@
     "CTkFont": {
         "Linux": {
             "family": "Roboto",
             "size": 13,
             "weight": "normal"
         },
         "Windows": {
-            "family": "Roboto",
-            "size": 13,
+            "family": "Microsoft YaHei",
+            "size": 12,
             "weight": "normal"
         },
         "macOS": {
             "family": "SF Display",
             "size": 13,
             "weight": "normal"
         }
@@ -280,28 +280,28 @@
         ],
         "progress_color": [
             "gray40",
             "#AAB0B5"
         ]
     },
     "CTkSwitch": {
-        "border_width": 1,
+        "border_width": 0.1,
         "button_color": [
             "#f3f3f3",
             "#000000"
         ],
         "button_hover_color": [
             "#bfbfbf",
             "#050505"
         ],
         "button_length": 0,
         "corner_radius": 1000,
         "fg_color": [
-            "#939BA2",
-            "#4A4D50"
+            "#ededed",
+            "#1d1d1d"
         ],
         "progress_color": [
             "#0067c0",
             "#4cc2ff"
         ],
         "text_color": [
             "gray10",
@@ -341,19 +341,19 @@
             "#ffffff",
             "#101010"
         ]
     },
     "DropdownMenu": {
         "fg_color": [
             "gray90",
-            "gray20"
+            "#1c1c1c"
         ],
         "hover_color": [
             "gray75",
-            "gray28"
+            "#313131"
         ],
         "text_color": [
             "gray10",
-            "gray90"
+            "#ffffff"
         ]
     }
 }
```

### Comparing `customtkinterx-0.1.3/customtkinterx/LaunchMusix.py` & `customtkinterx-0.1.4/customtkinterx/LaunchMusix.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.3/README.md` & `customtkinterx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.3/PKG-INFO` & `customtkinterx-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.1.3
+Version: 0.1.4
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

