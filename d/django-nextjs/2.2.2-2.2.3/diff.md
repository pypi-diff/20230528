# Comparing `tmp/django-nextjs-2.2.2.tar.gz` & `tmp/django-nextjs-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nextjs-2.2.2.tar", last modified: Thu Jan 12 20:39:41 2023, max compression
+gzip compressed data, was "django-nextjs-2.2.3.tar", last modified: Sun May 28 15:16:01 2023, max compression
```

## Comparing `django-nextjs-2.2.2.tar` & `django-nextjs-2.2.3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-01-12 20:39:41.397100 django-nextjs-2.2.2/
--rw-r--r--   0 danial    (1000) danial    (1000)     1076 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/LICENSE
--rw-r--r--   0 danial    (1000) danial    (1000)       62 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/MANIFEST.in
--rw-r--r--   0 danial    (1000) danial    (1000)     8973 2023-01-12 20:39:41.393767 django-nextjs-2.2.2/PKG-INFO
--rw-r--r--   0 danial    (1000) danial    (1000)     7914 2022-11-13 19:24:11.000000 django-nextjs-2.2.2/README.md
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-01-12 20:39:41.393767 django-nextjs-2.2.2/django_nextjs/
--rw-r--r--   0 danial    (1000) danial    (1000)       22 2023-01-12 20:38:44.000000 django-nextjs-2.2.2/django_nextjs/__init__.py
--rw-r--r--   0 danial    (1000) danial    (1000)      191 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/django_nextjs/app_settings.py
--rw-r--r--   0 danial    (1000) danial    (1000)      135 2022-09-16 11:04:07.000000 django-nextjs-2.2.2/django_nextjs/apps.py
--rw-r--r--   0 danial    (1000) danial    (1000)       54 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/django_nextjs/exceptions.py
--rw-r--r--   0 danial    (1000) danial    (1000)     3797 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/django_nextjs/proxy.py
--rw-r--r--   0 danial    (1000) danial    (1000)     5913 2023-01-12 20:37:05.000000 django-nextjs-2.2.2/django_nextjs/render.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-01-12 20:39:41.393767 django-nextjs-2.2.2/django_nextjs/templates/
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-01-12 20:39:41.393767 django-nextjs-2.2.2/django_nextjs/templates/django_nextjs/
--rw-r--r--   0 danial    (1000) danial    (1000)      246 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/django_nextjs/templates/django_nextjs/document_base.html
--rw-r--r--   0 danial    (1000) danial    (1000)      287 2022-03-05 14:42:22.000000 django-nextjs-2.2.2/django_nextjs/urls.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-01-12 20:39:41.393767 django-nextjs-2.2.2/django_nextjs.egg-info/
--rw-r--r--   0 danial    (1000) danial    (1000)     8973 2023-01-12 20:39:41.000000 django-nextjs-2.2.2/django_nextjs.egg-info/PKG-INFO
--rw-r--r--   0 danial    (1000) danial    (1000)      469 2023-01-12 20:39:41.000000 django-nextjs-2.2.2/django_nextjs.egg-info/SOURCES.txt
--rw-r--r--   0 danial    (1000) danial    (1000)        1 2023-01-12 20:39:41.000000 django-nextjs-2.2.2/django_nextjs.egg-info/dependency_links.txt
--rw-r--r--   0 danial    (1000) danial    (1000)      108 2023-01-12 20:39:41.000000 django-nextjs-2.2.2/django_nextjs.egg-info/requires.txt
--rw-r--r--   0 danial    (1000) danial    (1000)       14 2023-01-12 20:39:41.000000 django-nextjs-2.2.2/django_nextjs.egg-info/top_level.txt
--rw-r--r--   0 danial    (1000) danial    (1000)      281 2022-09-16 11:04:07.000000 django-nextjs-2.2.2/pyproject.toml
--rw-r--r--   0 danial    (1000) danial    (1000)       38 2023-01-12 20:39:41.397100 django-nextjs-2.2.2/setup.cfg
--rw-r--r--   0 danial    (1000) danial    (1000)     1802 2022-11-13 10:01:42.000000 django-nextjs-2.2.2/setup.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/
+-rw-r--r--   0 danial    (1000) danial    (1000)     1076 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/LICENSE
+-rw-r--r--   0 danial    (1000) danial    (1000)       62 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/MANIFEST.in
+-rw-r--r--   0 danial    (1000) danial    (1000)     8973 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/PKG-INFO
+-rw-r--r--   0 danial    (1000) danial    (1000)     7914 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/README.md
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.047196 django-nextjs-2.2.3/django_nextjs/
+-rw-r--r--   0 danial    (1000) danial    (1000)       22 2023-05-28 15:15:39.000000 django-nextjs-2.2.3/django_nextjs/__init__.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      191 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/app_settings.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      135 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/apps.py
+-rw-r--r--   0 danial    (1000) danial    (1000)       54 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/exceptions.py
+-rw-r--r--   0 danial    (1000) danial    (1000)     3797 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/proxy.py
+-rw-r--r--   0 danial    (1000) danial    (1000)     6347 2023-05-28 15:10:19.000000 django-nextjs-2.2.3/django_nextjs/render.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.047196 django-nextjs-2.2.3/django_nextjs/templates/
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/django_nextjs/templates/django_nextjs/
+-rw-r--r--   0 danial    (1000) danial    (1000)      246 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/templates/django_nextjs/document_base.html
+-rw-r--r--   0 danial    (1000) danial    (1000)      287 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/urls.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/django_nextjs.egg-info/
+-rw-r--r--   0 danial    (1000) danial    (1000)     8973 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/PKG-INFO
+-rw-r--r--   0 danial    (1000) danial    (1000)      490 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/SOURCES.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)        1 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/dependency_links.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)      108 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/requires.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)       14 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/top_level.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)      281 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/pyproject.toml
+-rw-r--r--   0 danial    (1000) danial    (1000)       38 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/setup.cfg
+-rw-r--r--   0 danial    (1000) danial    (1000)     1802 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/setup.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/tests/
+-rw-r--r--   0 danial    (1000) danial    (1000)     1119 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/tests/test_render.py
```

### Comparing `django-nextjs-2.2.2/LICENSE` & `django-nextjs-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-nextjs-2.2.2/PKG-INFO` & `django-nextjs-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nextjs
-Version: 2.2.2
+Version: 2.2.3
 Summary: Next.js + Django integration
 Home-page: https://github.com/QueraTeam/django-nextjs
 Download-URL: https://github.com/QueraTeam/django-nextjs
 Author: Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>
 Keywords: django,next,nextjs,django-nextjs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-nextjs-2.2.2/README.md` & `django-nextjs-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django-nextjs-2.2.2/django_nextjs/proxy.py` & `django-nextjs-2.2.3/django_nextjs/proxy.py`

 * *Files identical despite different names*

### Comparing `django-nextjs-2.2.2/django_nextjs/render.py` & `django-nextjs-2.2.3/django_nextjs/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,54 +27,58 @@
         "section4": html[c:d],
         "section5": html[d:],
     }
 
     return context
 
 
-def _get_cookies(request):
+def _get_cookies(request: HttpRequest):
     """
     Ensure we always send a CSRF cookie to Next.js server (if there is none in `request` object, generate one)
     Reason: We are going to issue GraphQL POST requests to fetch data in NextJS getServerSideProps.
             If this is the first request of user, there is no CSRF cookie and request fails,
             since GraphQL uses POST even for data fetching.
     Isn't this a vulnerability?
     No, as long as getServerSideProps functions are side effect free
     (i.e. dont use HTTP unsafe methods or GraphQL mutations).
     https://docs.djangoproject.com/en/3.2/ref/csrf/#is-posting-an-arbitrary-csrf-token-pair-cookie-and-post-data-a-vulnerability
     """
     return {**request.COOKIES, settings.CSRF_COOKIE_NAME: get_csrf_token(request)}
 
 
-def _get_headers(request):
+def _get_headers(request: HttpRequest, headers=None):
+    """
+    Headers that we will send in request to Next.js
+    """
     return {
         "x-real-ip": request.headers.get("X-Real-Ip", "") or request.META.get("REMOTE_ADDR", ""),
         "user-agent": request.headers.get("User-Agent", ""),
+        **({} if headers is None else headers),
     }
 
 
 def _get_nextjs_response_headers(headers):
     useful_header_keys = [
         "Location",
     ]
     return {key: headers[key] for key in useful_header_keys if key in headers}
 
 
 def _render_nextjs_page_to_string_sync(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False
+    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
 ) -> typing.Tuple[str, int, typing.Dict[str, str]]:
     page = requests.utils.quote(request.path_info.lstrip("/"))
     params = {k: request.GET.getlist(k) for k in request.GET.keys()}
 
     # Get HTML from Next.js server
     response = requests.get(
         f"{NEXTJS_SERVER_URL}/{page}",
         params=params,
         cookies=_get_cookies(request),
-        headers=_get_headers(request),
+        headers=_get_headers(request, headers),
         allow_redirects=allow_redirects,
     )
     html = response.text
     response_headers = _get_nextjs_response_headers(response.headers)
 
     # Apply template_name if provided
     if template_name:
@@ -82,47 +86,49 @@
         if final_context is not None:
             html = render_to_string(template_name, context=final_context, request=request, using=using)
 
     return html, response.status_code, response_headers
 
 
 def render_nextjs_page_to_string_sync(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False
+    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
 ) -> str:
     html, _, _ = _render_nextjs_page_to_string_sync(
-        request, template_name, context, using=using, allow_redirects=allow_redirects
+        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
     )
     return html
 
 
 def render_nextjs_page_sync(
     request: HttpRequest,
     template_name: str = "",
     context=None,
     content_type=None,
     override_status=None,
     using=None,
     allow_redirects=False,
+    headers=None,
 ) -> HttpResponse:
-    content, status, headers = _render_nextjs_page_to_string_sync(
-        request, template_name, context, using=using, allow_redirects=allow_redirects
+    content, status, response_headers = _render_nextjs_page_to_string_sync(
+        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
     )
-    return HttpResponse(content, content_type, status if override_status is None else override_status, headers=headers)
+    final_status = status if override_status is None else override_status
+    return HttpResponse(content, content_type, final_status, headers=response_headers)
 
 
 async def _render_nextjs_page_to_string_async(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False
+    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
 ) -> typing.Tuple[str, int, typing.Dict[str, str]]:
     page = requests.utils.quote(request.path_info.lstrip("/"))
     params = [(k, v) for k in request.GET.keys() for v in request.GET.getlist(k)]
 
     # Get HTML from Next.js server
     async with aiohttp.ClientSession(
         cookies=_get_cookies(request),
-        headers=_get_headers(request),
+        headers=_get_headers(request, headers),
     ) as session:
         async with session.get(
             f"{NEXTJS_SERVER_URL}/{page}", params=params, allow_redirects=allow_redirects
         ) as response:
             html = await response.text()
             response_headers = _get_nextjs_response_headers(response.headers)
 
@@ -133,28 +139,30 @@
             html = await sync_to_async(render_to_string)(
                 template_name, context=final_context, request=request, using=using
             )
     return html, response.status, response_headers
 
 
 async def render_nextjs_page_to_string_async(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False
+    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
 ) -> str:
     html, _, _ = await _render_nextjs_page_to_string_async(
-        request, template_name, context, using=using, allow_redirects=allow_redirects
+        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
     )
     return html
 
 
 async def render_nextjs_page_async(
     request: HttpRequest,
     template_name: str = "",
     context=None,
     content_type=None,
     override_status=None,
     using=None,
     allow_redirects=False,
+    headers=None,
 ) -> HttpResponse:
-    content, status, headers = await _render_nextjs_page_to_string_async(
-        request, template_name, context, using=using, allow_redirects=allow_redirects
+    content, status, response_headers = await _render_nextjs_page_to_string_async(
+        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
     )
-    return HttpResponse(content, content_type, status if override_status is None else override_status, headers=headers)
+    final_status = status if override_status is None else override_status
+    return HttpResponse(content, content_type, final_status, headers=response_headers)
```

### Comparing `django-nextjs-2.2.2/django_nextjs.egg-info/PKG-INFO` & `django-nextjs-2.2.3/django_nextjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nextjs
-Version: 2.2.2
+Version: 2.2.3
 Summary: Next.js + Django integration
 Home-page: https://github.com/QueraTeam/django-nextjs
 Download-URL: https://github.com/QueraTeam/django-nextjs
 Author: Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>
 Keywords: django,next,nextjs,django-nextjs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-nextjs-2.2.2/setup.py` & `django-nextjs-2.2.3/setup.py`

 * *Files identical despite different names*

