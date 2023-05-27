# Comparing `tmp/aiodiskqueue-0.1.0a6.tar.gz` & `tmp/aiodiskqueue-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0a8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a6.tar` & `aiodiskqueue-0.1.0a8.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a6/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a6/.github/workflows/main.yml
--rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a6/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a6/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     1967 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a6/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a6/docs/_static/custom.css
--rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a6/docs/api.rst
--rw-r--r--   0        0        0     1837 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a6/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a6/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a6/examples/__init__.py
--rw-r--r--   0        0        0      197 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/examples/basic_usage.py
--rw-r--r--   0        0        0      920 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/examples/multiple_consumers.py
--rw-r--r--   0        0        0      866 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/examples/single_consumer.py
--rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0      187 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     3793 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a6/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a6/tests/__init__.py
--rw-r--r--   0        0        0      514 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tests/factories.py
--rw-r--r--   0        0        0     3031 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tests/loadtest.py
--rw-r--r--   0        0        0     3033 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tests/test_core.py
--rw-r--r--   0        0        0      415 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tox.ini
--rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a8/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a8/.github/workflows/main.yml
+-rw-r--r--   0        0        0      113 2023-05-27 13:02:59.767723 aiodiskqueue-0.1.0a8/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a8/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a8/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-27 23:28:20.869763 aiodiskqueue-0.1.0a8/Makefile
+-rw-r--r--   0        0        0     2170 2023-05-27 23:17:03.567813 aiodiskqueue-0.1.0a8/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a8/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a8/docs/_static/custom.css
+-rw-r--r--   0        0        0      110 2023-05-27 23:22:27.264032 aiodiskqueue-0.1.0a8/docs/api.rst
+-rw-r--r--   0        0        0     1874 2023-05-27 23:26:37.783113 aiodiskqueue-0.1.0a8/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a8/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a8/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a8/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-27 21:27:48.522374 aiodiskqueue-0.1.0a8/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-27 22:42:54.736074 aiodiskqueue-0.1.0a8/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-27 22:43:05.224008 aiodiskqueue-0.1.0a8/examples/single_consumer.py
+-rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-05-27 22:41:31.268783 aiodiskqueue-0.1.0a8/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     7565 2023-05-27 23:20:25.643561 aiodiskqueue-0.1.0a8/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      268 2023-05-27 16:08:35.068771 aiodiskqueue-0.1.0a8/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a8/tests/__init__.py
+-rw-r--r--   0        0        0      514 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a8/tests/factories.py
+-rw-r--r--   0        0        0     3037 2023-05-27 22:56:42.848238 aiodiskqueue-0.1.0a8/tests/loadtest.py
+-rw-r--r--   0        0        0     6347 2023-05-27 22:39:35.585946 aiodiskqueue-0.1.0a8/tests/test_core.py
+-rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0a8/tox.ini
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a8/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a6/.github/workflows/main.yml` & `aiodiskqueue-0.1.0a8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a6/LICENSE` & `aiodiskqueue-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a6/README.rst` & `aiodiskqueue-0.1.0a8/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,43 +4,47 @@
 Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
-This library provides a persistent queue for Python AsyncIO.
+This library provides a persistent FIFO queue for Python AsyncIO:
 
-It has an API similar to the standard `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_,
-but items in the queue will persists between process restarts.
+- Queue content is preserved after a by process restart
+- Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
+- Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
+- Designed for durability and decent performance
+- Sane logging
+- Fully tested
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
 
     import asyncio
     from aiodiskqueue import Queue
 
     async def main():
-        q = Queue("example_queue.sqlite")
+        q = await Queue.create("example_queue.sqlite")
         await q.put("some item")
         item = await q.get()
         print(item)
 
     asyncio.run(main())
 
-Please see the examples folder for more usage examples.
+Please see the **examples** folder for more usage examples.
 
 Installation
 ------------
 
-You can install directly from PyPI with the following command:
+You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodiskqueue
```

### Comparing `aiodiskqueue-0.1.0a6/docs/Makefile` & `aiodiskqueue-0.1.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a6/docs/conf.py` & `aiodiskqueue-0.1.0a8/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 
 extensions = ["sphinx.ext.autodoc", "sphinx.ext.napoleon"]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for autodoc -----------------------------------------------------
-# autoclass_content = "both"
 autodoc_default_options = {
     "members": True,
     "member-order": "alphabetical",
     "undoc-members": False,
     "exclude-members": "__weakref__",
 }
+autoclass_content = "class"
+autodoc_class_signature = "separated"
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "alabaster"
 html_theme_options = {
     "description": "Persistent queue for Python AsyncIO",
```

### Comparing `aiodiskqueue-0.1.0a6/docs/make.bat` & `aiodiskqueue-0.1.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a6/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0a8/examples/multiple_consumers.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     while True:
         message = await queue.get()
         print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = Queue(path)
+    queue = await Queue.create(path)
     coroutines = [
         consumer(queue),
         consumer(queue),
         producer(queue, 1),
         producer(queue, 2),
         producer(queue, 3),
         producer(queue, 4),
```

### Comparing `aiodiskqueue-0.1.0a6/examples/single_consumer.py` & `aiodiskqueue-0.1.0a8/examples/single_consumer.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     while True:
         message = await queue.get()
         print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = Queue(path)
+    queue = await Queue.create(path)
     coroutines = [
         consumer(queue),
         producer(queue, 1),
         producer(queue, 2),
         producer(queue, 3),
     ]
     await asyncio.gather(*coroutines)
```

### Comparing `aiodiskqueue-0.1.0a6/pyproject.toml` & `aiodiskqueue-0.1.0a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a6/tests/factories.py` & `aiodiskqueue-0.1.0a8/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a6/tests/loadtest.py` & `aiodiskqueue-0.1.0a8/tests/loadtest.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 import aiodiskqueue
 
 logging.basicConfig(level="INFO", format="%(asctime)s - %(levelname)s -  %(message)s")
 
 logger = logging.getLogger(__name__)
 
-ITEMS_AMOUNT = 10000
-PRODUCER_AMOUNT = 50
+ITEMS_AMOUNT = 5000
+PRODUCER_AMOUNT = 100
 
 
 def random_string(length: int) -> str:
     return "".join(random.choices(string.ascii_uppercase + string.digits, k=length))
 
 
 async def producer(
@@ -43,41 +43,41 @@
 
 async def consumer(disk_queue: aiodiskqueue.Queue, result_queue: asyncio.Queue):
     logger.info("Starting consumer")
     try:
         while True:
             item = await disk_queue.get()
             await result_queue.put(item)
+            await disk_queue.task_done()
     except Exception:
         logger.exception("Consumer error")
 
 
 async def main(db_path):
     # create source queue with items
     items = [random_string(16) for _ in range(ITEMS_AMOUNT)]
     source_queue = asyncio.Queue()
     for item in items:
         source_queue.put_nowait(item)
 
     # create disk and destination queue
-    disk_queue = aiodiskqueue.Queue(db_path)
+    disk_queue = await aiodiskqueue.Queue.create(db_path, maxsize=1000)
     result_queue = asyncio.Queue()
 
     # start producer and consumers and wait for producers to finish
     start = time.perf_counter()
     consumer_task = asyncio.create_task(consumer(disk_queue, result_queue))
     producers = [
         producer(source_queue, disk_queue, num + 1) for num in range(PRODUCER_AMOUNT)
     ]
     await asyncio.gather(*producers)
 
     # wait for consumer to finish
     logger.info("Waiting for consumer to complete...")
-    while not await disk_queue.empty():
-        await asyncio.sleep(0.5)
+    await disk_queue.join()
     consumer_task.cancel()
 
     # measure duration and throughput
     duration = time.perf_counter() - start
     throughput = ITEMS_AMOUNT * 2 / duration
     logger.info("Duration: %f seconds, queue ops per sec: %f", duration, throughput)
 
@@ -99,8 +99,7 @@
 
     logger.info("Peak size of disk queue was: %d", disk_queue._peak_size)
 
 
 db_path = Path(__file__).parent / "loadtest_queue.dat"
 db_path.unlink(missing_ok=True)
 asyncio.run(main(db_path))
-db_path.unlink()
```

### Comparing `aiodiskqueue-0.1.0a6/PKG-INFO` & `aiodiskqueue-0.1.0a8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a6
+Version: 0.1.0a8
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -23,43 +23,47 @@
 Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
-This library provides a persistent queue for Python AsyncIO.
+This library provides a persistent FIFO queue for Python AsyncIO:
 
-It has an API similar to the standard `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_,
-but items in the queue will persists between process restarts.
+- Queue content is preserved after a by process restart
+- Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
+- Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
+- Designed for durability and decent performance
+- Sane logging
+- Fully tested
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
 
     import asyncio
     from aiodiskqueue import Queue
 
     async def main():
-        q = Queue("example_queue.sqlite")
+        q = await Queue.create("example_queue.sqlite")
         await q.put("some item")
         item = await q.get()
         print(item)
 
     asyncio.run(main())
 
-Please see the examples folder for more usage examples.
+Please see the **examples** folder for more usage examples.
 
 Installation
 ------------
 
-You can install directly from PyPI with the following command:
+You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodiskqueue
```

