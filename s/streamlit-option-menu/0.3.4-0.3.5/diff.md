# Comparing `tmp/streamlit-option-menu-0.3.4.tar.gz` & `tmp/streamlit-option-menu-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-option-menu-0.3.4.tar", last modified: Wed May 17 16:19:49 2023, max compression
+gzip compressed data, was "streamlit-option-menu-0.3.5.tar", last modified: Sun May 28 10:16:54 2023, max compression
```

## Comparing `streamlit-option-menu-0.3.4.tar` & `streamlit-option-menu-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/
--rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       56 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2430 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     4694 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2769 2023-05-17 16:18:28.000000 streamlit-option-menu-0.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/
--rwxr-xr-x   0 root         (0) root         (0)     4284 2023-05-17 15:34:56.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/app.9b0f7d0b.css
--rw-r--r--   0 root         (0) root         (0)   273142 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)   164360 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff
--rw-r--r--   0 root         (0) root         (0)   121340 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/
--rw-r--r--   0 root         (0) root         (0)     7352 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js
--rw-r--r--   0 root         (0) root         (0)    28619 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js.map
--rw-r--r--   0 root         (0) root         (0)   328486 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js
--rw-r--r--   0 root         (0) root         (0)  1616052 2023-05-17 16:19:27.000000 streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:19:49.508247 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2430 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      860 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 16:19:49.000000 streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/
+-rwxr-xr-x   0 root         (0) root         (0)     1074 2023-05-17 16:28:00.000000 streamlit-option-menu-0.3.5/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       56 2023-05-17 16:28:00.000000 streamlit-option-menu-0.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     4693 2023-05-17 16:52:14.000000 streamlit-option-menu-0.3.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2769 2023-05-28 10:14:07.000000 streamlit-option-menu-0.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.561860 streamlit-option-menu-0.3.5/streamlit_option_menu/
+-rwxr-xr-x   0 root         (0) root         (0)     4284 2023-05-17 16:28:00.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.561860 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/css/
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/css/app.731d875d.css
+-rw-r--r--   0 root         (0) root         (0)   273142 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)   164360 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff
+-rw-r--r--   0 root         (0) root         (0)   121340 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/
+-rw-r--r--   0 root         (0) root         (0)     7370 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/app.3d75d26b.js
+-rw-r--r--   0 root         (0) root         (0)    28612 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/app.3d75d26b.js.map
+-rw-r--r--   0 root         (0) root         (0)   328486 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js
+-rw-r--r--   0 root         (0) root         (0)  1616052 2023-05-28 10:16:29.000000 streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 10:16:54.571860 streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-05-28 10:16:54.000000 streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      860 2023-05-28 10:16:54.000000 streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 10:16:54.000000 streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-28 10:16:54.000000 streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-28 10:16:54.000000 streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/top_level.txt
```

### Comparing `streamlit-option-menu-0.3.4/LICENSE` & `streamlit-option-menu-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/PKG-INFO` & `streamlit-option-menu-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-option-menu
-Version: 0.3.4
+Version: 0.3.5
 Summary: streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.
 Home-page: https://github.com/victoryhb/streamlit-option-menu
 Author: Victor Yan
 Author-email: victoryhb@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `streamlit-option-menu-0.3.4/README.md` & `streamlit-option-menu-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,19 +34,17 @@
     * "nav-link-selected": the &lt;a> element containing the text of the selected option
     * "icon": the icon next to each option
     * "separator": the &lt;hr> element separating the options
 - manual_select: Pass to manually change the menu item selection. 
 The function returns the (string) option currently selected
 
 ### Manual Selection
-This option was added in order to let the user manually move to a specific option in the menu. This could come in handy where when finished with one option and want to move the user automatically to another option (For example if approved setings, then  move back to main option)
+This option was added to allow the user to manually move to a specific option in the menu. This could be useful when the user wants to move to another option automatically after finishing with one option (for example, if settings are approved, then move back to the main option).
 
-In order to use this option, you need to pass the index of the wanted option as a `manual_select`.
-
-<br>**Notice** -  This acts like a button, meaning you should only pass the manual_select once when wanting to "click" the option, and not keep it as a constant value to your menu creation call (see example below).
+To use this option, you need to pass the index of the desired option as `manual_select`. **Notice**: This option behaves like a button. This means that you should only pass `manual_select` once when you want to select the option, and not keep it as a constant value in your menu creation call (see example below).
 
 
 ## Examples
 ```
 import streamlit as st
 from streamlit_option_menu import option_menu
```

### Comparing `streamlit-option-menu-0.3.4/setup.py` & `streamlit-option-menu-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-option-menu",
-    version="0.3.4",
+    version="0.3.5",
     author="Victor Yan",
     author_email="victoryhb@163.com",
     description="streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.",
     long_description="""streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.
 It is similar in function to st.selectbox(), except that:
 - It uses a simple static list to display the options instead of a dropdown
 - It has configurable icons for each option item and the menu title
```

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/__init__.py` & `streamlit-option-menu-0.3.5/streamlit_option_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/app.3d75d26b.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 (function(e) {
     function t(t) {
-        for (var r, s, a = t[0], i = t[1], l = t[2], b = 0, j = []; b < a.length; b++) s = a[b], Object.prototype.hasOwnProperty.call(c, s) && c[s] && j.push(c[s][0]), c[s] = 0;
-        for (r in i) Object.prototype.hasOwnProperty.call(i, r) && (e[r] = i[r]);
+        for (var r, s, i = t[0], a = t[1], l = t[2], b = 0, j = []; b < i.length; b++) s = i[b], Object.prototype.hasOwnProperty.call(c, s) && c[s] && j.push(c[s][0]), c[s] = 0;
+        for (r in a) Object.prototype.hasOwnProperty.call(a, r) && (e[r] = a[r]);
         u && u(t);
         while (j.length) j.shift()();
         return o.push.apply(o, l || []), n()
     }
 
     function n() {
         for (var e, t = 0; t < o.length; t++) {
-            for (var n = o[t], r = !0, a = 1; a < n.length; a++) {
-                var i = n[a];
-                0 !== c[i] && (r = !1)
+            for (var n = o[t], r = !0, i = 1; i < n.length; i++) {
+                var a = n[i];
+                0 !== c[a] && (r = !1)
             }
             r && (o.splice(t--, 1), e = s(s.s = n[0]))
         }
         return e
     }
     var r = {},
         c = {
@@ -61,67 +61,63 @@
         } : function() {
             return e
         };
         return s.d(t, "a", t), t
     }, s.o = function(e, t) {
         return Object.prototype.hasOwnProperty.call(e, t)
     }, s.p = "";
-    var a = window["webpackJsonp"] = window["webpackJsonp"] || [],
-        i = a.push.bind(a);
-    a.push = t, a = a.slice();
-    for (var l = 0; l < a.length; l++) t(a[l]);
-    var u = i;
+    var i = window["webpackJsonp"] = window["webpackJsonp"] || [],
+        a = i.push.bind(i);
+    i.push = t, i = i.slice();
+    for (var l = 0; l < i.length; l++) t(i[l]);
+    var u = a;
     o.push([0, "chunk-vendors"]), n()
 })({
     0: function(e, t, n) {
         e.exports = n("cd49")
     },
     "04d9": function(e, t, n) {
         "use strict";
         n("7746")
     },
     "44dc": function(e, t, n) {
         "use strict";
         n("a61a")
     },
     7746: function(e, t, n) {},
-    8972: function(e, t, n) {
-        "use strict";
-        n("ea33")
-    },
     a61a: function(e, t, n) {},
     cd49: function(e, t, n) {
         "use strict";
         n.r(t);
         var r = n("7a23");
         const c = {
             id: "app"
         };
 
-        function o(e, t, n, o, s, a) {
-            const i = Object(r["u"])("MyComponent"),
+        function o(e, t, n, o, s, i) {
+            const a = Object(r["u"])("MyComponent"),
                 l = Object(r["u"])("WithStreamlitConnection");
             return Object(r["o"])(), Object(r["d"])("div", c, [Object(r["g"])(l, null, {
                 default: Object(r["x"])(({
                     args: e
-                }) => [Object(r["g"])(i, {
+                }) => [Object(r["g"])(a, {
                     args: e
                 }, null, 8, ["args"])]),
                 _: 1
             })])
         }
-        const s = e => (Object(r["q"])("data-v-ef155198"), e = e(), Object(r["p"])(), e),
-            a = {
+        const s = e => (Object(r["q"])("data-v-448f46e8"), e = e(), Object(r["p"])(), e),
+            i = {
                 class: "menu"
             },
-            i = s(() => Object(r["e"])("hr", null, null, -1)),
+            a = s(() => Object(r["e"])("hr", null, null, -1)),
             l = ["onClick"];
 
         function u(e, t, n, c, o, s) {
-            return Object(r["o"])(), Object(r["d"])("div", a, [Object(r["e"])("div", {
+            return Object(r["o"])(), Object(r["d"])("div", i, [Object(r["e"])("div", {
                 class: Object(r["i"])(["container-xxl d-flex flex-column flex-shrink-0", {
                     "p-3": !c.isHorizontal,
                     "p-h": c.isHorizontal,
                     "nav-justified": c.isHorizontal
                 }]),
                 style: Object(r["j"])(c.styleObjectToString(c.styles["container"]))
             }, [c.menuTitle ? (Object(r["o"])(), Object(r["d"])(r["a"], {
@@ -129,15 +125,15 @@
             }, [Object(r["e"])("a", {
                 href: "#",
                 class: "menu-title align-items-center mb-md-0 me-md-auto text-decoration-none",
                 style: Object(r["j"])(c.styleObjectToString(c.styles["menu-title"]))
             }, [Object(r["e"])("i", {
                 class: Object(r["i"])(["icon", c.menuIcon]),
                 style: Object(r["j"])(c.styleObjectToString(c.styles["menu-icon"]))
-            }, null, 6), Object(r["f"])(" " + Object(r["v"])(c.menuTitle), 1)], 4), i], 64)) : Object(r["c"])("", !0), Object(r["e"])("ul", {
+            }, null, 6), Object(r["f"])(" " + Object(r["v"])(c.menuTitle), 1)], 4), a], 64)) : Object(r["c"])("", !0), Object(r["e"])("ul", {
                 class: Object(r["i"])(["nav nav-pills mb-auto", {
                     "flex-column": !c.isHorizontal,
                     "nav-justified": c.isHorizontal
                 }]),
                 style: Object(r["j"])(c.styleObjectToString(c.styles["nav"]))
             }, [(Object(r["o"])(!0), Object(r["d"])(r["a"], null, Object(r["s"])(n.args.options, (e, t) => (Object(r["o"])(), Object(r["d"])("li", {
                 class: "nav-item",
@@ -147,15 +143,15 @@
                 key: 0,
                 class: Object(r["i"])({
                     vr: c.isHorizontal
                 }),
                 style: Object(r["j"])(c.styleObjectToString(c.styles["separator"]))
             }, null, 6)) : (Object(r["o"])(), Object(r["d"])("a", {
                 key: 1,
-                href: "#",
+                href: "javascript:void(0);",
                 class: Object(r["i"])(["nav-link", {
                     active: t == c.selectedIndex,
                     "nav-link-horizontal": c.isHorizontal
                 }]),
                 onClick: n => c.onClicked(t, e),
                 "aria-current": "page",
                 style: Object(r["j"])(c.styleObjectToString(c.styles["nav-link"]) + c.styleObjectToString(c.styles["nav-link-selected"], t == c.selectedIndex))
@@ -187,62 +183,62 @@
          * distributed under the License is distributed on an "AS IS" BASIS,
          * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
          * See the License for the specific language governing permissions and
          * limitations under the License.
          */
         n("ab8b"), n("cd74");
 
-        function O(e) {
+        function d(e) {
             return "bi-" !== e.slice(0, 3) ? "bi-" + e : e
         }
-        var d = {
+        var O = {
                 name: "MyComponent",
                 props: ["args"],
                 setup(e) {
                     j();
                     const t = Object(r["r"])(e.args.menuTitle),
                         n = "horizontal" == e.args.orientation,
                         c = Object(r["r"])(e.args.menuIcon || "bi-menu-up");
-                    c.value = O(c.value);
+                    c.value = d(c.value);
                     const o = Object(r["r"])(e.args.icons || []);
-                    for (let r = 0; r < e.args.options.length; r++) o.value[r] || (o.value[r] = "bi-caret-right"), o.value[r] = O(o.value[r]);
+                    for (let r = 0; r < e.args.options.length; r++) o.value[r] || (o.value[r] = "bi-caret-right"), o.value[r] = d(o.value[r]);
                     const s = Object(r["r"])(e.args.defaultIndex),
-                        a = (e, t) => {
+                        i = (e, t) => {
                             s.value = e, b["a"].setComponentValue(t)
                         },
-                        i = (e, t) => {
+                        a = (e, t) => {
                             if ("undefined" === typeof t && (t = !0), !t) return "";
                             let n = "";
                             for (const r in e) n += `${r}:${e[r]};`;
                             return n
                         },
                         l = Object(r["r"])(e.args.styles || {}),
                         u = t => {
-                            console.log("chosen index is: ", t), t >= 0 && t < e.args.options.length ? a(t, e.args.options[t]) : console.warn("Invalid index for triggerMenuClick")
+                            console.log("chosen index is: ", t), t >= 0 && t < e.args.options.length ? i(t, e.args.options[t]) : console.warn("Invalid index for triggerMenuClick")
                         };
                     return Object(r["w"])(() => e.args.manualSelect, (t, n) => {
-                        void 0 !== t && null !== t && t !== n && a(t, e.args.options[t])
+                        void 0 !== t && null !== t && t !== n && i(t, e.args.options[t])
                     }), {
                         triggerMenuClick: u,
                         selectedIndex: s,
                         menuTitle: t,
                         menuIcon: c,
                         icons: o,
                         styles: l,
-                        onClicked: a,
-                        styleObjectToString: i,
+                        onClicked: i,
+                        styleObjectToString: a,
                         isHorizontal: n
                     }
                 }
             },
-            p = (n("8972"), n("6b0d")),
+            p = (n("fce6"), n("6b0d")),
             f = n.n(p);
-        const v = f()(d, [
+        const v = f()(O, [
             ["render", u],
-            ["__scopeId", "data-v-ef155198"]
+            ["__scopeId", "data-v-448f46e8"]
         ]);
         var g = v;
         const y = e => (Object(r["q"])("data-v-bef81972"), e = e(), Object(r["p"])(), e),
             m = {
                 key: 0
             },
             h = y(() => Object(r["e"])("h1", {
@@ -298,10 +294,14 @@
         n("04d9");
         const E = f()(C, [
             ["render", o]
         ]);
         var w = E;
         Object(r["b"])(w).mount("#app")
     },
-    ea33: function(e, t, n) {}
+    d4cd: function(e, t, n) {},
+    fce6: function(e, t, n) {
+        "use strict";
+        n("d4cd")
+    }
 });
-//# sourceMappingURL=app.625674d3.js.map
+//# sourceMappingURL=app.3d75d26b.js.map
```

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/app.625674d3.js.map` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/app.3d75d26b.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8016917293233082%*

 * *Differences: {"'file'": "'js/app.3d75d26b.js'",*

 * * "'mappings'": "'aACE,SAASA,EAAqBC,GAQ7B,IAPA,IAMIC,EAAUC,EANVC,EAAWH,EAAK,GAChBI,EAAcJ,EAAK,GACnBK,EAAiBL,EAAK,GAIHM,EAAI,EAAGC,EAAW,GACpCD,EAAIH,EAASK,OAAQF,IACzBJ,EAAUC,EAASG,GAChBG,OAAOC,UAAUC,eAAeC,KAAKC,EAAiBX,IAAYW,EAAgBX,IACpFK,EAASO,KAAKD,EAAgBX,GAAS,IAExCW,EAAgBX,GAAW,EAE5B,IAAID,KAAYG,EACZK,OAAOC,UAAUC,eAAeC,KAAKR,EAAaH,KACpDc,EAAQd,GAAYG,EAAYH,IAG/Be,GAAqBA,EAAoBhB,GAE5C,MAAMO,EAASC,OACdD,EAASU,OAATV,GAOD,OAHAW,EAAgBJ,KAAKK,MAAMD,EAAiBb,GAAkB,IAGvDe,IAER,SAASA, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "js/app.625674d3.js",
-    "mappings": "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",
+    "file": "js/app.3d75d26b.js",
+    "mappings": "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",
     "names": [
         "webpackJsonpCallback",
         "data",
         "moduleId",
         "chunkId",
         "chunkIds",
         "moreModules",
@@ -166,37 +166,37 @@
         "mount"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///webpack/bootstrap",
         "webpack:///./src/App.vue?6a6e",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?df18",
-        "webpack:///./src/MyComponent.vue?2b86",
         "webpack:///./src/App.vue?5a4f",
         "webpack:///./src/MyComponent.vue",
         "webpack:///./src/streamlit/StreamlitVue.ts",
         "webpack:///./src/MyComponent.vue?82ad",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?82f3",
-        "webpack:///./src/streamlit/WithStreamlitConnection.vue?15eb",
+        "webpack:///./src/streamlit/WithStreamlitConnection.vue",
         "webpack:///./src/streamlit/WithStreamlitConnection.vue?22ba",
         "webpack:///./src/App.vue?47b3",
         "webpack:///./src/App.vue?8ecf",
-        "webpack:///./src/main.ts"
+        "webpack:///./src/main.ts",
+        "webpack:///./src/MyComponent.vue?79a3"
     ],
     "sourcesContent": [
         " \t// install a JSONP callback for chunk loading\n \tfunction webpackJsonpCallback(data) {\n \t\tvar chunkIds = data[0];\n \t\tvar moreModules = data[1];\n \t\tvar executeModules = data[2];\n\n \t\t// add \"moreModules\" to the modules object,\n \t\t// then flag all \"chunkIds\" as loaded and fire callback\n \t\tvar moduleId, chunkId, i = 0, resolves = [];\n \t\tfor(;i < chunkIds.length; i++) {\n \t\t\tchunkId = chunkIds[i];\n \t\t\tif(Object.prototype.hasOwnProperty.call(installedChunks, chunkId) && installedChunks[chunkId]) {\n \t\t\t\tresolves.push(installedChunks[chunkId][0]);\n \t\t\t}\n \t\t\tinstalledChunks[chunkId] = 0;\n \t\t}\n \t\tfor(moduleId in moreModules) {\n \t\t\tif(Object.prototype.hasOwnProperty.call(moreModules, moduleId)) {\n \t\t\t\tmodules[moduleId] = moreModules[moduleId];\n \t\t\t}\n \t\t}\n \t\tif(parentJsonpFunction) parentJsonpFunction(data);\n\n \t\twhile(resolves.length) {\n \t\t\tresolves.shift()();\n \t\t}\n\n \t\t// add entry modules from loaded chunk to deferred list\n \t\tdeferredModules.push.apply(deferredModules, executeModules || []);\n\n \t\t// run deferred modules when all chunks ready\n \t\treturn checkDeferredModules();\n \t};\n \tfunction checkDeferredModules() {\n \t\tvar result;\n \t\tfor(var i = 0; i < deferredModules.length; i++) {\n \t\t\tvar deferredModule = deferredModules[i];\n \t\t\tvar fulfilled = true;\n \t\t\tfor(var j = 1; j < deferredModule.length; j++) {\n \t\t\t\tvar depId = deferredModule[j];\n \t\t\t\tif(installedChunks[depId] !== 0) fulfilled = false;\n \t\t\t}\n \t\t\tif(fulfilled) {\n \t\t\t\tdeferredModules.splice(i--, 1);\n \t\t\t\tresult = __webpack_require__(__webpack_require__.s = deferredModule[0]);\n \t\t\t}\n \t\t}\n\n \t\treturn result;\n \t}\n\n \t// The module cache\n \tvar installedModules = {};\n\n \t// object to store loaded and loading chunks\n \t// undefined = chunk not loaded, null = chunk preloaded/prefetched\n \t// Promise = chunk loading, 0 = chunk loaded\n \tvar installedChunks = {\n \t\t\"app\": 0\n \t};\n\n \tvar deferredModules = [];\n\n \t// The require function\n \tfunction __webpack_require__(moduleId) {\n\n \t\t// Check if module is in cache\n \t\tif(installedModules[moduleId]) {\n \t\t\treturn installedModules[moduleId].exports;\n \t\t}\n \t\t// Create a new module (and put it into the cache)\n \t\tvar module = installedModules[moduleId] = {\n \t\t\ti: moduleId,\n \t\t\tl: false,\n \t\t\texports: {}\n \t\t};\n\n \t\t// Execute the module function\n \t\tmodules[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n \t\t// Flag the module as loaded\n \t\tmodule.l = true;\n\n \t\t// Return the exports of the module\n \t\treturn module.exports;\n \t}\n\n\n \t// expose the modules object (__webpack_modules__)\n \t__webpack_require__.m = modules;\n\n \t// expose the module cache\n \t__webpack_require__.c = installedModules;\n\n \t// define getter function for harmony exports\n \t__webpack_require__.d = function(exports, name, getter) {\n \t\tif(!__webpack_require__.o(exports, name)) {\n \t\t\tObject.defineProperty(exports, name, { enumerable: true, get: getter });\n \t\t}\n \t};\n\n \t// define __esModule on exports\n \t__webpack_require__.r = function(exports) {\n \t\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n \t\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n \t\t}\n \t\tObject.defineProperty(exports, '__esModule', { value: true });\n \t};\n\n \t// create a fake namespace object\n \t// mode & 1: value is a module id, require it\n \t// mode & 2: merge all properties of value into the ns\n \t// mode & 4: return value when already ns object\n \t// mode & 8|1: behave like require\n \t__webpack_require__.t = function(value, mode) {\n \t\tif(mode & 1) value = __webpack_require__(value);\n \t\tif(mode & 8) return value;\n \t\tif((mode & 4) && typeof value === 'object' && value && value.__esModule) return value;\n \t\tvar ns = Object.create(null);\n \t\t__webpack_require__.r(ns);\n \t\tObject.defineProperty(ns, 'default', { enumerable: true, value: value });\n \t\tif(mode & 2 && typeof value != 'string') for(var key in value) __webpack_require__.d(ns, key, function(key) { return value[key]; }.bind(null, key));\n \t\treturn ns;\n \t};\n\n \t// getDefaultExport function for compatibility with non-harmony modules\n \t__webpack_require__.n = function(module) {\n \t\tvar getter = module && module.__esModule ?\n \t\t\tfunction getDefault() { return module['default']; } :\n \t\t\tfunction getModuleExports() { return module; };\n \t\t__webpack_require__.d(getter, 'a', getter);\n \t\treturn getter;\n \t};\n\n \t// Object.prototype.hasOwnProperty.call\n \t__webpack_require__.o = function(object, property) { return Object.prototype.hasOwnProperty.call(object, property); };\n\n \t// __webpack_public_path__\n \t__webpack_require__.p = \"\";\n\n \tvar jsonpArray = window[\"webpackJsonp\"] = window[\"webpackJsonp\"] || [];\n \tvar oldJsonpFunction = jsonpArray.push.bind(jsonpArray);\n \tjsonpArray.push = webpackJsonpCallback;\n \tjsonpArray = jsonpArray.slice();\n \tfor(var i = 0; i < jsonpArray.length; i++) webpackJsonpCallback(jsonpArray[i]);\n \tvar parentJsonpFunction = oldJsonpFunction;\n\n\n \t// add entry module to deferred list\n \tdeferredModules.push([0,\"chunk-vendors\"]);\n \t// run deferred modules when ready\n \treturn checkDeferredModules();\n",
         "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--7-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--7-oneOf-1-1!../node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--7-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--1-0!../node_modules/vue-loader-v16/dist/index.js??ref--1-1!./App.vue?vue&type=style&index=0&id=07d8329a&lang=css\"",
         "export * from \"-!../../node_modules/mini-css-extract-plugin/dist/loader.js??ref--7-oneOf-1-0!../../node_modules/css-loader/dist/cjs.js??ref--7-oneOf-1-1!../../node_modules/vue-loader-v16/dist/stylePostLoader.js!../../node_modules/postcss-loader/src/index.js??ref--7-oneOf-1-2!../../node_modules/cache-loader/dist/cjs.js??ref--1-0!../../node_modules/vue-loader-v16/dist/index.js??ref--1-1!./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"",
-        "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--7-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--7-oneOf-1-1!../node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--7-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--1-0!../node_modules/vue-loader-v16/dist/index.js??ref--1-1!./MyComponent.vue?vue&type=style&index=0&id=ef155198&scoped=true&lang=css\"",
         "import { resolveComponent as _resolveComponent, createVNode as _createVNode, withCtx as _withCtx, openBlock as _openBlock, createElementBlock as _createElementBlock } from \"vue\"\n\nconst _hoisted_1 = { id: \"app\" }\n\nexport function render(_ctx: any,_cache: any,$props: any,$setup: any,$data: any,$options: any) {\n  const _component_MyComponent = _resolveComponent(\"MyComponent\")!\n  const _component_WithStreamlitConnection = _resolveComponent(\"WithStreamlitConnection\")!\n\n  return (_openBlock(), _createElementBlock(\"div\", _hoisted_1, [\n    _createVNode(_component_WithStreamlitConnection, null, {\n      default: _withCtx(({ args }) => [\n        _createVNode(_component_MyComponent, { args: args }, null, 8, [\"args\"])\n      ]),\n      _: 1\n    })\n  ]))\n}",
-        "<template>\n    <div class=\"menu\">\n        <div class=\"container-xxl d-flex flex-column flex-shrink-0\" :class=\"{'p-3': !isHorizontal, 'p-h':isHorizontal, 'nav-justified': isHorizontal}\" :style=\"styleObjectToString(styles['container'])\">\n            <template v-if=\"menuTitle\">\n                <a href=\"#\" class=\"menu-title align-items-center mb-md-0 me-md-auto text-decoration-none\"\n                :style=\"styleObjectToString(styles['menu-title'])\"\n                >\n                    <i class=\"icon\" :class=\"menuIcon\" :style=\"styleObjectToString(styles['menu-icon'])\"></i>\n                    {{menuTitle}}\n                </a>\n            <hr>\n            </template>\n            <ul class=\"nav nav-pills mb-auto\" :class=\"{'flex-column': !isHorizontal, 'nav-justified': isHorizontal}\"\n            :style=\"styleObjectToString(styles['nav'])\"\n            >\n                <li class=\"nav-item\" v-for=\"(option,i) in args.options\" :key=\"option\"\n                :style=\"styleObjectToString(styles['nav-item'])\"\n                >\n                    <hr :class=\"{vr: isHorizontal}\" v-if=\"option === '---'\" :style=\"styleObjectToString(styles['separator'])\">\n                    <a v-else href=\"#\" class=\"nav-link\" :class=\"{active: i == selectedIndex, 'nav-link-horizontal':isHorizontal}\" \n                    @click=\"onClicked(i, option)\" aria-current=\"page\" \n                    :style=\"styleObjectToString(styles['nav-link']) + styleObjectToString(styles['nav-link-selected'], i == selectedIndex)\">\n                        <i class=\"icon\" :class=\"icons[i]\" :style=\"styleObjectToString(styles['icon'])\"></i>\n                        {{option}}\n                    </a>\n                </li>\n            </ul>\n        </div>\n    </div>\n</template>\n<script>\nimport { ref, watch } from \"vue\"\nimport { Streamlit } from \"streamlit-component-lib\"\nimport { useStreamlit } from \"./streamlit\"\nimport \"bootstrap/dist/css/bootstrap.min.css\"\nimport \"bootstrap-icons/font/bootstrap-icons.css\";\n\n\nfunction getFullIconName(name) {\n    return name.slice(0,3) !== \"bi-\"? \"bi-\" + name : name\n}\n\nexport default {\n    name: \"MyComponent\",\n    props: [\"args\"], // Arguments that are passed to the plugin in Python are accessible in prop \"args\"\n    setup(props) {\n        useStreamlit() // lifecycle hooks for automatic Streamlit resize\n\n        const menuTitle = ref(props.args.menuTitle)\n        const isHorizontal = props.args.orientation == \"horizontal\"\n        const menuIcon = ref(props.args.menuIcon || \"bi-menu-up\")\n        menuIcon.value = getFullIconName(menuIcon.value)\n        const icons = ref(props.args.icons || [])\n        for (let i = 0; i < props.args.options.length; i++) {\n            if (!icons.value[i]) {\n                icons.value[i] = \"bi-caret-right\";\n            }\n            icons.value[i] = getFullIconName(icons.value[i]);\n        }\n        const selectedIndex = ref(props.args.defaultIndex)\n        const onClicked = (index, option) => {\n            selectedIndex.value = index\n            Streamlit.setComponentValue(option)\n        }\n        const styleObjectToString = (obj, condition) => {\n            if (typeof condition === \"undefined\") {\n                condition = true\n            }\n            if (!condition) {\n                return \"\"\n            }\n            let styleString = \"\"\n            for (const key in obj) {\n                styleString += `${key}:${obj[key]};`\n            }\n            return styleString\n        }\n        const styles = ref(props.args.styles || {});\n        // const manualSelect = props.args.manualSelect === undefined || props.args.manualSelect === null ? NaN : props.args.manualSelect;\n        \n        const triggerMenuClick = (index) => {\n            console.log(\"chosen index is: \", index)\n            if (index >= 0 && index < props.args.options.length) {\n                onClicked(index, props.args.options[index]);\n            } else {\n                console.warn('Invalid index for triggerMenuClick');\n            }\n        }\n\n\n        watch(\n            () => props.args.manualSelect,\n            (newClickPos, oldClickPos) => {\n                if (newClickPos !== undefined && newClickPos !== null && newClickPos !== oldClickPos) {\n                onClicked(newClickPos, props.args.options[newClickPos])\n                }\n            }\n        )\n\n        return {\n            triggerMenuClick,\n            selectedIndex,\n            menuTitle,\n            menuIcon,\n            icons,\n            styles,\n            onClicked,\n            styleObjectToString,\n            isHorizontal\n        }\n    },\n}\n</script>\n\n<style scoped>\n.icon {\n    font-size: 1rem;\n    margin-right: 0.5rem;\n}\n\n.menu hr {\n    margin-top: 0.5rem;\n    margin-bottom: 0.5rem;\n}\n\n.menu .container-xxl {\n   background-color: var(--secondary-background-color);\n   border-radius: 0.5rem;\n}\n\n.menu-title {\n    margin-left: 0.75rem;\n    margin-right: 0.75rem;\n}\n\n.menu-title, .menu-title .icon {\n    font-size: 1.5rem;\n}\n\n.menu-title .icon {\n    margin-right: 0.75rem;\n}\n\n.menu-title, .menu .nav-link, .menu .nav-item, hr {\n    color: var(--text-color);\n}\n\n.nav-link.active {\n    color: white;\n}\n\n.nav-link:hover {\n    background-color: var(--hover-color);\n}\n\n.nav-link-hover:hover {\n    background-color: inherit;\n}\n\n.menu .nav-link {\n    /* box-shadow: 0 0px 0.2rem #aaa; */\n    margin-top: 0.25rem;\n    margin-bottom: 0.25rem;\n    padding-top: 0.5rem;\n    padding-bottom: 0.5rem;\n}\n\n.menu .nav-link-horizontal {\n    /* margin-top: 0.25rem;\n    margin-bottom: 0.25rem; */\n    padding-top: 0.25rem;\n    padding-bottom: 0.25rem;\n}\n\n.p-h {\n    padding: 0.5rem 0.75rem;\n}\n\n.container .flex-column {\n    padding-top: 0.25rem;\n}\n\n.menu .nav-item .nav-link.active{\n    background-color: var(--primary-color);\n}\n\n.nav-link.active, .nav-link.active+.icon {\n    font-weight: 900;\n}\n\n.vr {\n    width: 1px; \n    height: 80%;\n}\n</style>\n",
+        "<template>\n    <div class=\"menu\">\n        <div class=\"container-xxl d-flex flex-column flex-shrink-0\" :class=\"{'p-3': !isHorizontal, 'p-h':isHorizontal, 'nav-justified': isHorizontal}\" :style=\"styleObjectToString(styles['container'])\">\n            <template v-if=\"menuTitle\">\n                <a href=\"#\" class=\"menu-title align-items-center mb-md-0 me-md-auto text-decoration-none\"\n                :style=\"styleObjectToString(styles['menu-title'])\"\n                >\n                    <i class=\"icon\" :class=\"menuIcon\" :style=\"styleObjectToString(styles['menu-icon'])\"></i>\n                    {{menuTitle}}\n                </a>\n            <hr>\n            </template>\n            <ul class=\"nav nav-pills mb-auto\" :class=\"{'flex-column': !isHorizontal, 'nav-justified': isHorizontal}\"\n            :style=\"styleObjectToString(styles['nav'])\"\n            >\n                <li class=\"nav-item\" v-for=\"(option,i) in args.options\" :key=\"option\"\n                :style=\"styleObjectToString(styles['nav-item'])\"\n                >\n                    <hr :class=\"{vr: isHorizontal}\" v-if=\"option === '---'\" :style=\"styleObjectToString(styles['separator'])\">\n                    <a v-else href=\"javascript:void(0);\" class=\"nav-link\" :class=\"{active: i == selectedIndex, 'nav-link-horizontal':isHorizontal}\" \n                    @click=\"onClicked(i, option)\" aria-current=\"page\" \n                    :style=\"styleObjectToString(styles['nav-link']) + styleObjectToString(styles['nav-link-selected'], i == selectedIndex)\">\n                        <i class=\"icon\" :class=\"icons[i]\" :style=\"styleObjectToString(styles['icon'])\"></i>\n                        {{option}}\n                    </a>\n                </li>\n            </ul>\n        </div>\n    </div>\n</template>\n<script>\nimport { ref, watch } from \"vue\"\nimport { Streamlit } from \"streamlit-component-lib\"\nimport { useStreamlit } from \"./streamlit\"\nimport \"bootstrap/dist/css/bootstrap.min.css\"\nimport \"bootstrap-icons/font/bootstrap-icons.css\";\n\n\nfunction getFullIconName(name) {\n    return name.slice(0,3) !== \"bi-\"? \"bi-\" + name : name\n}\n\nexport default {\n    name: \"MyComponent\",\n    props: [\"args\"], // Arguments that are passed to the plugin in Python are accessible in prop \"args\"\n    setup(props) {\n        useStreamlit() // lifecycle hooks for automatic Streamlit resize\n\n        const menuTitle = ref(props.args.menuTitle)\n        const isHorizontal = props.args.orientation == \"horizontal\"\n        const menuIcon = ref(props.args.menuIcon || \"bi-menu-up\")\n        menuIcon.value = getFullIconName(menuIcon.value)\n        const icons = ref(props.args.icons || [])\n        for (let i = 0; i < props.args.options.length; i++) {\n            if (!icons.value[i]) {\n                icons.value[i] = \"bi-caret-right\";\n            }\n            icons.value[i] = getFullIconName(icons.value[i]);\n        }\n        const selectedIndex = ref(props.args.defaultIndex)\n        const onClicked = (index, option) => {\n            selectedIndex.value = index\n            Streamlit.setComponentValue(option)\n        }\n        const styleObjectToString = (obj, condition) => {\n            if (typeof condition === \"undefined\") {\n                condition = true\n            }\n            if (!condition) {\n                return \"\"\n            }\n            let styleString = \"\"\n            for (const key in obj) {\n                styleString += `${key}:${obj[key]};`\n            }\n            return styleString\n        }\n        const styles = ref(props.args.styles || {});\n        // const manualSelect = props.args.manualSelect === undefined || props.args.manualSelect === null ? NaN : props.args.manualSelect;\n        \n        const triggerMenuClick = (index) => {\n            console.log(\"chosen index is: \", index)\n            if (index >= 0 && index < props.args.options.length) {\n                onClicked(index, props.args.options[index]);\n            } else {\n                console.warn('Invalid index for triggerMenuClick');\n            }\n        }\n\n\n        watch(\n            () => props.args.manualSelect,\n            (newClickPos, oldClickPos) => {\n                if (newClickPos !== undefined && newClickPos !== null && newClickPos !== oldClickPos) {\n                onClicked(newClickPos, props.args.options[newClickPos])\n                }\n            }\n        )\n\n        return {\n            triggerMenuClick,\n            selectedIndex,\n            menuTitle,\n            menuIcon,\n            icons,\n            styles,\n            onClicked,\n            styleObjectToString,\n            isHorizontal\n        }\n    },\n}\n</script>\n\n<style scoped>\n.icon {\n    font-size: 1rem;\n    margin-right: 0.5rem;\n}\n\n.menu hr {\n    margin-top: 0.5rem;\n    margin-bottom: 0.5rem;\n}\n\n.menu .container-xxl {\n   background-color: var(--secondary-background-color);\n   border-radius: 0.5rem;\n}\n\n.menu-title {\n    margin-left: 0.75rem;\n    margin-right: 0.75rem;\n}\n\n.menu-title, .menu-title .icon {\n    font-size: 1.5rem;\n}\n\n.menu-title .icon {\n    margin-right: 0.75rem;\n}\n\n.menu-title, .menu .nav-link, .menu .nav-item, hr {\n    color: var(--text-color);\n}\n\n.nav-link.active {\n    color: white;\n}\n\n.nav-link:hover {\n    background-color: var(--hover-color);\n}\n\n.nav-link-hover:hover {\n    background-color: inherit;\n}\n\n.menu .nav-link {\n    /* box-shadow: 0 0px 0.2rem #aaa; */\n    margin-top: 0.25rem;\n    margin-bottom: 0.25rem;\n    padding-top: 0.5rem;\n    padding-bottom: 0.5rem;\n}\n\n.menu .nav-link-horizontal {\n    /* margin-top: 0.25rem;\n    margin-bottom: 0.25rem; */\n    padding-top: 0.25rem;\n    padding-bottom: 0.25rem;\n}\n\n.p-h {\n    padding: 0.5rem 0.75rem;\n}\n\n.container .flex-column {\n    padding-top: 0.25rem;\n}\n\n.menu .nav-item .nav-link.active{\n    background-color: var(--primary-color);\n}\n\n.nav-link.active, .nav-link.active+.icon {\n    font-weight: 900;\n}\n\n.vr {\n    width: 1px; \n    height: 80%;\n}\n</style>\n",
         "/**\n * Vue.js specific composables\n */\nimport { onMounted, onUpdated } from \"vue\"\nimport { Streamlit } from \"streamlit-component-lib\"\n\nexport function useStreamlit() {\n  /**\n   * Optional Streamlit Vue-based setup.\n   *\n   * You are not required call this function on your Streamlit\n   * component. If you decide not to call it, you should implement the\n   * `onMounted` and `onUpdated` functions in your own component,\n   * so that your plugin properly resizes.\n   */\n\n  onMounted((): void => {\n    // After we're rendered for the first time, tell Streamlit that our height\n    // has changed.\n    Streamlit.setFrameHeight()\n  })\n\n  onUpdated((): void => {\n    // After we're updated, tell Streamlit that our height may have changed.\n    Streamlit.setFrameHeight()\n  })\n}\n",
-        "import { render } from \"./MyComponent.vue?vue&type=template&id=ef155198&scoped=true\"\nimport script from \"./MyComponent.vue?vue&type=script&lang=js\"\nexport * from \"./MyComponent.vue?vue&type=script&lang=js\"\n\nimport \"./MyComponent.vue?vue&type=style&index=0&id=ef155198&scoped=true&lang=css\"\n\nimport exportComponent from \"/root/code/streamlit-option-menu-master/streamlit_option_menu/frontend/node_modules/vue-loader-v16/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render],['__scopeId',\"data-v-ef155198\"]])\n\nexport default __exports__",
+        "import { render } from \"./MyComponent.vue?vue&type=template&id=448f46e8&scoped=true\"\nimport script from \"./MyComponent.vue?vue&type=script&lang=js\"\nexport * from \"./MyComponent.vue?vue&type=script&lang=js\"\n\nimport \"./MyComponent.vue?vue&type=style&index=0&id=448f46e8&scoped=true&lang=css\"\n\nimport exportComponent from \"/root/code/streamlit-option-menu/streamlit_option_menu/frontend/node_modules/vue-loader-v16/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render],['__scopeId',\"data-v-448f46e8\"]])\n\nexport default __exports__",
         "import { createElementVNode as _createElementVNode, toDisplayString as _toDisplayString, openBlock as _openBlock, createElementBlock as _createElementBlock, createCommentVNode as _createCommentVNode, renderSlot as _renderSlot, pushScopeId as _pushScopeId, popScopeId as _popScopeId } from \"vue\"\n\nconst _withScopeId = n => (_pushScopeId(\"data-v-bef81972\"),n=n(),_popScopeId(),n)\nconst _hoisted_1 = { key: 0 }\nconst _hoisted_2 = /*#__PURE__*/ _withScopeId(() => /*#__PURE__*/_createElementVNode(\"h1\", { class: \"err__title\" }, \"Component Error\", -1))\nconst _hoisted_3 = { class: \"err__msg\" }\n\nexport function render(_ctx: any,_cache: any,$props: any,$setup: any,$data: any,$options: any) {\n  return (_openBlock(), _createElementBlock(\"div\", null, [\n    (_ctx.componentError != '')\n      ? (_openBlock(), _createElementBlock(\"div\", _hoisted_1, [\n          _hoisted_2,\n          _createElementVNode(\"div\", _hoisted_3, \"Message: \" + _toDisplayString(_ctx.componentError), 1)\n        ]))\n      : (_ctx.renderData != null)\n        ? _renderSlot(_ctx.$slots, \"default\", {\n            key: 1,\n            args: _ctx.renderData.args,\n            disabled: _ctx.renderData.disabled\n          }, undefined, true)\n        : _createCommentVNode(\"\", true)\n  ]))\n}",
         "\nimport {\n  ref,\n  defineComponent,\n  onMounted,\n  onUpdated,\n  onUnmounted,\n  onErrorCaptured,\n} from \"vue\"\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nexport default defineComponent({\n  name: \"WithStreamlitConnection\",\n  setup() {\n    const renderData = ref<RenderData>((undefined as unknown) as RenderData)\n    const componentError = ref(\"\")\n\n    const onRenderEvent = (event: Event): void => {\n      const renderEvent = event as CustomEvent<RenderData>\n      renderData.value = renderEvent.detail\n      componentError.value = \"\"\n    }\n\n    // Set up event listeners, and signal to Streamlit that we're ready.\n    // We won't render the component until we receive the first RENDER_EVENT.\n    onMounted(() => {\n      Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRenderEvent)\n      Streamlit.setComponentReady()\n    })\n    onUpdated(() => {\n      // If our slot threw an error, we display it in render(). In this\n      // case, the slot won't be mounted and therefore won't call\n      // `setFrameHeight` on its own. We do it here so that the rendered\n      // error will be visible.\n      if (componentError.value != \"\") {\n        Streamlit.setFrameHeight()\n      }\n    })\n    onUnmounted(() => {\n      Streamlit.events.removeEventListener(\n        Streamlit.RENDER_EVENT,\n        onRenderEvent\n      )\n    })\n    onErrorCaptured(err => {\n      componentError.value = String(err)\n    })\n\n    return {\n      renderData,\n      componentError,\n    }\n  },\n})\n",
-        "import { render } from \"./WithStreamlitConnection.vue?vue&type=template&id=bef81972&scoped=true&ts=true\"\nimport script from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\nexport * from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\n\nimport \"./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"\n\nimport exportComponent from \"/root/code/streamlit-option-menu-master/streamlit_option_menu/frontend/node_modules/vue-loader-v16/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render],['__scopeId',\"data-v-bef81972\"]])\n\nexport default __exports__",
+        "import { render } from \"./WithStreamlitConnection.vue?vue&type=template&id=bef81972&scoped=true&ts=true\"\nimport script from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\nexport * from \"./WithStreamlitConnection.vue?vue&type=script&lang=ts\"\n\nimport \"./WithStreamlitConnection.vue?vue&type=style&index=0&id=bef81972&scoped=true&lang=css\"\n\nimport exportComponent from \"/root/code/streamlit-option-menu/streamlit_option_menu/frontend/node_modules/vue-loader-v16/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render],['__scopeId',\"data-v-bef81972\"]])\n\nexport default __exports__",
         "\nimport { defineComponent } from \"vue\"\nimport MyComponent from \"./MyComponent.vue\"\n\n// \"withStreamlitConnection\" is a scoped slot. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nimport WithStreamlitConnection from \"./streamlit/WithStreamlitConnection.vue\"\n\nexport default defineComponent({\n  name: \"App\",\n  components: {\n    MyComponent,\n    WithStreamlitConnection,\n  },\n})\n",
-        "import { render } from \"./App.vue?vue&type=template&id=07d8329a&ts=true\"\nimport script from \"./App.vue?vue&type=script&lang=ts\"\nexport * from \"./App.vue?vue&type=script&lang=ts\"\n\nimport \"./App.vue?vue&type=style&index=0&id=07d8329a&lang=css\"\n\nimport exportComponent from \"/root/code/streamlit-option-menu-master/streamlit_option_menu/frontend/node_modules/vue-loader-v16/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render]])\n\nexport default __exports__",
-        "import { createApp } from 'vue'\nimport App from './App.vue'\n\ncreateApp(App).mount('#app')\n"
+        "import { render } from \"./App.vue?vue&type=template&id=07d8329a&ts=true\"\nimport script from \"./App.vue?vue&type=script&lang=ts\"\nexport * from \"./App.vue?vue&type=script&lang=ts\"\n\nimport \"./App.vue?vue&type=style&index=0&id=07d8329a&lang=css\"\n\nimport exportComponent from \"/root/code/streamlit-option-menu/streamlit_option_menu/frontend/node_modules/vue-loader-v16/dist/exportHelper.js\"\nconst __exports__ = /*#__PURE__*/exportComponent(script, [['render',render]])\n\nexport default __exports__",
+        "import { createApp } from 'vue'\nimport App from './App.vue'\n\ncreateApp(App).mount('#app')\n",
+        "export * from \"-!../node_modules/mini-css-extract-plugin/dist/loader.js??ref--7-oneOf-1-0!../node_modules/css-loader/dist/cjs.js??ref--7-oneOf-1-1!../node_modules/vue-loader-v16/dist/stylePostLoader.js!../node_modules/postcss-loader/src/index.js??ref--7-oneOf-1-2!../node_modules/cache-loader/dist/cjs.js??ref--1-0!../node_modules/vue-loader-v16/dist/index.js??ref--1-1!./MyComponent.vue?vue&type=style&index=0&id=448f46e8&scoped=true&lang=css\""
     ],
     "version": 3
 }
```

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map` & `streamlit-option-menu-0.3.5/streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/PKG-INFO` & `streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-option-menu
-Version: 0.3.4
+Version: 0.3.5
 Summary: streamlit-option-menu is a simple Streamlit component that allows users to select a single item from a list of options in a menu.
 Home-page: https://github.com/victoryhb/streamlit-option-menu
 Author: Victor Yan
 Author-email: victoryhb@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `streamlit-option-menu-0.3.4/streamlit_option_menu.egg-info/SOURCES.txt` & `streamlit-option-menu-0.3.5/streamlit_option_menu.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 streamlit_option_menu/__init__.py
 streamlit_option_menu.egg-info/PKG-INFO
 streamlit_option_menu.egg-info/SOURCES.txt
 streamlit_option_menu.egg-info/dependency_links.txt
 streamlit_option_menu.egg-info/requires.txt
 streamlit_option_menu.egg-info/top_level.txt
 streamlit_option_menu/frontend/dist/index.html
-streamlit_option_menu/frontend/dist/css/app.9b0f7d0b.css
+streamlit_option_menu/frontend/dist/css/app.731d875d.css
 streamlit_option_menu/frontend/dist/css/chunk-vendors.89b53d14.css
 streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.3d0ec57f.woff
 streamlit_option_menu/frontend/dist/fonts/bootstrap-icons.a30fb81b.woff2
-streamlit_option_menu/frontend/dist/js/app.625674d3.js
-streamlit_option_menu/frontend/dist/js/app.625674d3.js.map
+streamlit_option_menu/frontend/dist/js/app.3d75d26b.js
+streamlit_option_menu/frontend/dist/js/app.3d75d26b.js.map
 streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js
 streamlit_option_menu/frontend/dist/js/chunk-vendors.a2e4d9cb.js.map
```

