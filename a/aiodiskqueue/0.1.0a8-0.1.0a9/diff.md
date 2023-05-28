# Comparing `tmp/aiodiskqueue-0.1.0a8.tar.gz` & `tmp/aiodiskqueue-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0a9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a8.tar` & `aiodiskqueue-0.1.0a9.tar`

### file list

```diff
@@ -1,28 +1,33 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a8/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a8/.github/workflows/main.yml
--rw-r--r--   0        0        0      113 2023-05-27 13:02:59.767723 aiodiskqueue-0.1.0a8/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a8/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a8/LICENSE
--rw-r--r--   0        0        0      121 2023-05-27 23:28:20.869763 aiodiskqueue-0.1.0a8/Makefile
--rw-r--r--   0        0        0     2170 2023-05-27 23:17:03.567813 aiodiskqueue-0.1.0a8/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a8/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a8/docs/_static/custom.css
--rw-r--r--   0        0        0      110 2023-05-27 23:22:27.264032 aiodiskqueue-0.1.0a8/docs/api.rst
--rw-r--r--   0        0        0     1874 2023-05-27 23:26:37.783113 aiodiskqueue-0.1.0a8/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a8/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a8/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a8/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-27 21:27:48.522374 aiodiskqueue-0.1.0a8/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-27 22:42:54.736074 aiodiskqueue-0.1.0a8/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-27 22:43:05.224008 aiodiskqueue-0.1.0a8/examples/single_consumer.py
--rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-27 22:41:31.268783 aiodiskqueue-0.1.0a8/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     7565 2023-05-27 23:20:25.643561 aiodiskqueue-0.1.0a8/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      268 2023-05-27 16:08:35.068771 aiodiskqueue-0.1.0a8/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a8/tests/__init__.py
--rw-r--r--   0        0        0      514 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a8/tests/factories.py
--rw-r--r--   0        0        0     3037 2023-05-27 22:56:42.848238 aiodiskqueue-0.1.0a8/tests/loadtest.py
--rw-r--r--   0        0        0     6347 2023-05-27 22:39:35.585946 aiodiskqueue-0.1.0a8/tests/test_core.py
--rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0a8/tox.ini
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a9/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a9/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0a9/.github/workflows/release.yml
+-rw-r--r--   0        0        0      113 2023-05-28 13:27:18.116278 aiodiskqueue-0.1.0a9/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a9/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0a9/Makefile
+-rw-r--r--   0        0        0     2170 2023-05-28 14:06:56.935356 aiodiskqueue-0.1.0a9/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a9/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a9/docs/_static/custom.css
+-rw-r--r--   0        0        0      110 2023-05-28 18:07:59.394553 aiodiskqueue-0.1.0a9/docs/api.rst
+-rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0a9/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a9/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a9/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a9/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0a9/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0a9/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0a9/examples/single_consumer.py
+-rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0a9/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     7836 2023-05-28 18:28:49.530087 aiodiskqueue-0.1.0a9/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0a9/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0a9/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a9/tests/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0a9/tests/factories.py
+-rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0a9/tests/helpers.py
+-rw-r--r--   0        0        0     3158 2023-05-28 14:06:56.951355 aiodiskqueue-0.1.0a9/tests/loadtest.py
+-rw-r--r--   0        0        0     6476 2023-05-28 18:50:55.148916 aiodiskqueue-0.1.0a9/tests/test_core.py
+-rw-r--r--   0        0        0     2493 2023-05-28 18:39:49.776986 aiodiskqueue-0.1.0a9/tests/test_integration.py
+-rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0a9/tests/test_utils.py
+-rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0a9/tox.ini
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a9/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a8/.github/workflows/main.yml` & `aiodiskqueue-0.1.0a9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/LICENSE` & `aiodiskqueue-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/README.rst` & `aiodiskqueue-0.1.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/docs/Makefile` & `aiodiskqueue-0.1.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/docs/conf.py` & `aiodiskqueue-0.1.0a9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for autodoc -----------------------------------------------------
 autodoc_default_options = {
     "members": True,
     "member-order": "alphabetical",
     "undoc-members": False,
-    "exclude-members": "__weakref__",
+    "exclude-members": "__weakref__, __init__",
 }
 autoclass_content = "class"
 autodoc_class_signature = "separated"
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `aiodiskqueue-0.1.0a8/docs/make.bat` & `aiodiskqueue-0.1.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0a9/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/examples/single_consumer.py` & `aiodiskqueue-0.1.0a9/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/pyproject.toml` & `aiodiskqueue-0.1.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a8/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0a9/src/aiodiskqueue/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from pathlib import Path
 from typing import Any, Union
 
 import aiofiles
 import aiofiles.os
 
 from aiodiskqueue.exceptions import QueueEmpty, QueueFull
+from aiodiskqueue.utils import NoDirectInstantiation
 
 logger = logging.getLogger(__name__)
 
 
-class Queue:
+class Queue(metaclass=NoDirectInstantiation):
     """A persistent AsyncIO FIFO queue.
 
     The content of a queue is stored on disk in a data file.
     This file usually only exists temporarily while there are items in the queue.
 
     An existing data file is used to recreate a queue,
     e.g. to preserve the queue content after a process restart
@@ -26,19 +27,23 @@
     so the queue can continue to function normally.
 
     Using two different instances with the same data file simultaneously
     is not recommended as it may lead to data corruption.
 
     This class is not thread safe.
 
-    Create a queue with the factory method :func:`create`.
+    To create a new object the factory method :func:`create` must be used.
     """
 
     def __init__(self, data_path: Path, maxsize: int, queue: list) -> None:
-        """:meta private:"""
+        """Direct instantiation would break the persistance feature
+        and has therefore been disabled.
+
+        :meta private:
+        """
         self._data_path = Path(data_path)
         self._maxsize = max(0, maxsize)
         self._queue_lock = asyncio.Lock()
         self._has_new_item = asyncio.Condition()
         self._has_free_slots = asyncio.Condition()
         self._tasks_are_finished = asyncio.Condition()
         self._unfinished_tasks = 0
@@ -170,15 +175,17 @@
                 raise ValueError("task_done() called too many times")
 
             self._unfinished_tasks -= 1
             if self._unfinished_tasks == 0:
                 self._tasks_are_finished.notify_all()
 
     async def _write_queue(self):
-        async with aiofiles.open(self._data_path, "wb", buffering=0) as fp:
+        async with aiofiles.open(
+            self._data_path, "wb", buffering=0
+        ) as fp:  # buffering is disabled to prevent the unclosed file issue.
             await fp.write(pickle.dumps(self._queue))
         size = self.qsize()
         self._peak_size = max(self._peak_size, size)
         logger.debug("Wrote queue with %d items: %s", size, self._data_path)
 
     @staticmethod
     async def _read_queue(data_path: Path) -> list:
@@ -190,28 +197,27 @@
 
         try:
             queue = pickle.loads(data)
         except pickle.PickleError:
             logger.exception("Data file is corrupt. Will be discarded: %s", data_path)
             return []
 
-        if queue:
-            logger.info(
-                "Resurrecting queue with %d items from file: %s",
-                len(queue),
-                data_path,
-            )
+        logger.info(
+            "Resurrecting queue with %d items from file: %s",
+            len(queue),
+            data_path,
+        )
         return queue
 
     @classmethod
     async def create(cls, data_path: Union[str, Path], maxsize: int = 0) -> "Queue":
         """Create a queue.
 
         Args:
             data_path: Path of the data file for this queue. e.g. `queue.dat`
             maxsize: If maxsize is less than or equal to zero, the queue size is infinite.
                 If it is an integer greater than 0, then put() blocks
                 when the queue reaches maxsize until an item is removed by get().
         """
         data_path = Path(data_path)
         queue = await cls._read_queue(data_path)
-        return cls(data_path, maxsize, queue)
+        return cls._create(data_path, maxsize, queue)
```

### Comparing `aiodiskqueue-0.1.0a8/tests/factories.py` & `aiodiskqueue-0.1.0a9/tests/factories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime as dt
 from dataclasses import dataclass
 
 import factory
 import factory.fuzzy
 
 
-@dataclass
+@dataclass(frozen=True)
 class Item:
     """An item for testing the queue."""
 
     message: str
     timestamp: dt.datetime
     volume: float
```

### Comparing `aiodiskqueue-0.1.0a8/tests/loadtest.py` & `aiodiskqueue-0.1.0a9/tests/loadtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Load testing the Queue.
 
-Runs many producers and 1 consumer in parallel and measures duration and throughput.
+Runs multiple producers and consumers in parallel and measures duration and throughput.
 
 For each item one put and one get is performed = 2 queue operations.
 """
 
 import asyncio
 import logging
 import random
@@ -16,14 +16,16 @@
 
 logging.basicConfig(level="INFO", format="%(asctime)s - %(levelname)s -  %(message)s")
 
 logger = logging.getLogger(__name__)
 
 ITEMS_AMOUNT = 5000
 PRODUCER_AMOUNT = 100
+CONSUMER_AMOUNT = 2
+DISKQUEUE_MAXSIZE = 1000
 
 
 def random_string(length: int) -> str:
     return "".join(random.choices(string.ascii_uppercase + string.digits, k=length))
 
 
 async def producer(
@@ -34,72 +36,76 @@
         try:
             item = source_queue.get_nowait()
         except asyncio.QueueEmpty:
             logger.info("Stopping producer %d", num)
             return
         else:
             await disk_queue.put(item)
-            await asyncio.sleep(random.random() / 10)
 
 
 async def consumer(disk_queue: aiodiskqueue.Queue, result_queue: asyncio.Queue):
     logger.info("Starting consumer")
     try:
         while True:
             item = await disk_queue.get()
             await result_queue.put(item)
             await disk_queue.task_done()
     except Exception:
         logger.exception("Consumer error")
 
 
-async def main(db_path):
-    # create source queue with items
-    items = [random_string(16) for _ in range(ITEMS_AMOUNT)]
+async def main(data_path):
+    # create queues
     source_queue = asyncio.Queue()
-    for item in items:
-        source_queue.put_nowait(item)
-
-    # create disk and destination queue
-    disk_queue = await aiodiskqueue.Queue.create(db_path, maxsize=1000)
+    disk_queue = await aiodiskqueue.Queue.create(data_path, maxsize=DISKQUEUE_MAXSIZE)
     result_queue = asyncio.Queue()
 
+    # create source queue with items
+    source_items = {random_string(16) for _ in range(ITEMS_AMOUNT)}
+    for item in source_items:
+        source_queue.put_nowait(item)
+
     # start producer and consumers and wait for producers to finish
     start = time.perf_counter()
-    consumer_task = asyncio.create_task(consumer(disk_queue, result_queue))
+    consumer_tasks = [
+        asyncio.create_task(consumer(disk_queue, result_queue))
+        for _ in range(CONSUMER_AMOUNT)
+    ]
     producers = [
         producer(source_queue, disk_queue, num + 1) for num in range(PRODUCER_AMOUNT)
     ]
     await asyncio.gather(*producers)
 
     # wait for consumer to finish
     logger.info("Waiting for consumer to complete...")
     await disk_queue.join()
-    consumer_task.cancel()
+    end = time.perf_counter()
+    for task in consumer_tasks:
+        task.cancel()
 
     # measure duration and throughput
-    duration = time.perf_counter() - start
+    duration = end - start
     throughput = ITEMS_AMOUNT * 2 / duration
     logger.info("Duration: %f seconds, queue ops per sec: %f", duration, throughput)
 
     # compare source items with result items
-    items_2 = []
+    result_items = set()
     while True:
         try:
             item = result_queue.get_nowait()
         except asyncio.QueueEmpty:
             break
         else:
-            items_2.append(item)
-    dif = set(items).difference(set(items_2))
+            result_items.add(item)
+    dif = source_items.difference(result_items)
     if not dif:
         logger.info("OK")
     else:
         logger.error("Differences found")
         logger.info("dif: %s", sorted(list(dif)))
 
     logger.info("Peak size of disk queue was: %d", disk_queue._peak_size)
 
 
-db_path = Path(__file__).parent / "loadtest_queue.dat"
-db_path.unlink(missing_ok=True)
-asyncio.run(main(db_path))
+data_path = Path(__file__).parent / "loadtest_queue.dat"
+data_path.unlink(missing_ok=True)
+asyncio.run(main(data_path))
```

### Comparing `aiodiskqueue-0.1.0a8/tests/test_core.py` & `aiodiskqueue-0.1.0a9/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,109 @@
 import asyncio
-import shutil
-import tempfile
-import unittest
-from pathlib import Path
 
 import aiofiles
 
 from aiodiskqueue import Queue, QueueEmpty, QueueFull
 
 from .factories import ItemFactory
+from .helpers import QueueAsyncioTestCase
 
 
-class TestQueue(unittest.IsolatedAsyncioTestCase):
-    def setUp(self) -> None:
-        self.temp_dir = Path(tempfile.mkdtemp())
-        self.data_path = self.temp_dir / "queue.dat"
+class TestCreateQueue(QueueAsyncioTestCase):
+    async def test_should_create_queue_and_measure_size(self):
+        # given
+        q = await Queue.create(self.data_path)
+        # when/then
+        self.assertIsInstance(q, Queue)
 
-    def tearDown(self) -> None:
-        shutil.rmtree(self.temp_dir, ignore_errors=True)
+    def test_should_raise_error_when_trying_to_instantiate_directly(self):
+        # when/then
+        with self.assertRaises(TypeError):
+            Queue()
 
-    async def test_should_create_queue_and_measure_size(self):
+    async def test_creating_queue_with_maxsize_below_0_yields_unlimited_queue(self):
+        # when
+        q = await Queue.create(self.data_path, maxsize=-1)
+        # then
+        self.assertEqual(q.maxsize, 0)
+
+    async def test_should_create_new_file_when_current_file_is_corrupt(self):
         # given
+        async with aiofiles.open(self.data_path, "wb") as fp:
+            await fp.write(b"invalid-data")
         q = await Queue.create(self.data_path)
         # when
         result = q.qsize()
         # then
         self.assertEqual(result, 0)
 
+    async def test_should_preserve_queue_content(self):
+        # given
+        queue_1 = await Queue.create(self.data_path)
+        item = ItemFactory()
+        await queue_1.put_nowait(item)
+        # when
+        del queue_1
+        queue_2 = await Queue.create(self.data_path)
+        item_new = await queue_2.get()
+        # then
+        self.assertEqual(item_new, item)
+
+
+class TestPutIntoQueue(QueueAsyncioTestCase):
     async def test_should_put_items_and_measure_size(self):
         # given
         q = await Queue.create(self.data_path)
         # when
         await q.put_nowait(ItemFactory())
         await q.put_nowait(ItemFactory())
         # then
         result = q.qsize()
         self.assertEqual(result, 2)
 
+    async def test_should_delete_file_when_queue_is_empty(self):
+        # given
+        q = await Queue.create(self.data_path)
+        await q.put_nowait(ItemFactory)
+        # when
+        await q.get()
+        # then
+        self.assertFalse(self.data_path.exists())
+
+    async def test_should_raise_error_when_putting_into_full_queue(self):
+        # given
+        q = await Queue.create(self.data_path, maxsize=1)
+        await q.put_nowait(ItemFactory)
+        # when
+        with self.assertRaises(QueueFull):
+            await q.put_nowait(ItemFactory)
+
+    async def test_put_should_block_until_queue_has_free_slots(self):
+        async def producer(item):
+            await q.put(item)
+
+        async def consumer():
+            return await q.get()
+
+        # given
+        q = await Queue.create(self.data_path, maxsize=1)
+        await q.put_nowait("item-1")
+
+        # when
+        producer_task = asyncio.create_task(producer("item-2"))
+        await asyncio.sleep(1)  # producer sees a full queue when task starts
+        consumer_task = asyncio.create_task(consumer())
+        await asyncio.gather(producer_task, consumer_task)
+
+        item = await q.get_nowait()
+        # then
+        self.assertEqual(item, "item-2")
+
+
+class TestRetrieveFromQueue(QueueAsyncioTestCase):
     async def test_should_get_item(self):
         # given
         q = await Queue.create(self.data_path)
         item = ItemFactory()
         await q.put_nowait(item)
         await q.put_nowait(ItemFactory())
         # when
@@ -51,66 +114,43 @@
     async def test_should_raise_exception_when_get_on_empty_queue(self):
         # given
         q = await Queue.create(self.data_path)
         # when/then
         with self.assertRaises(QueueEmpty):
             await q.get_nowait()
 
-    async def test_should_report_as_empty(self):
-        # given
-        q = await Queue.create(self.data_path)
-        # when/then
-        self.assertTrue(q.empty())
-
-    async def test_should_not_report_as_empty(self):
-        # given
-        q = await Queue.create(self.data_path)
-        await q.put_nowait(ItemFactory())
-        # when/then
-        self.assertFalse(q.empty())
-
     async def test_get_should_wait_until_item_is_available(self):
         async def consumer():
-            item = await q.get()
-            await queue_2.put(item)
+            item = await input_queue.get()
+            await result_queue.put(item)
 
         # given
-        queue_2 = asyncio.Queue()
-        q = await Queue.create(self.data_path)
+        input_queue = await Queue.create(self.data_path)
+        result_queue = asyncio.Queue()
         asyncio.create_task(consumer())
         # when
         await asyncio.sleep(1)  # consumer sees an empty queue when task starts
         item = ItemFactory()
-        await q.put_nowait(item)
+        await input_queue.put_nowait(item)
         # then
-        item_new = await queue_2.get()
+        item_new = await result_queue.get()
         self.assertEqual(item_new, item)
 
-    async def test_should_create_new_file_when_current_file_is_corrupt(self):
+    async def test_should_raise_error_when_calling_task_done_too_often(self):
         # given
-        async with aiofiles.open(self.data_path, "wb") as fp:
-            await fp.write(b"invalid-data")
         q = await Queue.create(self.data_path)
-        # when
-        result = q.qsize()
-        # then
-        self.assertEqual(result, 0)
+        await q.put_nowait(ItemFactory)
+        await q.get()
+        await q.task_done()
+        # when/then
+        with self.assertRaises(ValueError):
+            await q.task_done()
 
-    async def test_should_preserve_queue_content(self):
-        # given
-        queue_1 = await Queue.create(self.data_path)
-        item = ItemFactory()
-        await queue_1.put_nowait(item)
-        # when
-        del queue_1
-        queue_2 = await Queue.create(self.data_path)
-        item_new = await queue_2.get()
-        # then
-        self.assertEqual(item_new, item)
 
+class TestWaitUntilQueueIsEmpty(QueueAsyncioTestCase):
     async def test_join_should_block_until_all_tasks_completed(self):
         async def consumer(queue: Queue):
             while True:
                 await queue.get()
                 await queue.task_done()
 
         # given
@@ -122,67 +162,34 @@
         # when
         await queue.join()
         # then
         consumer_task.cancel()
         result = queue.empty()
         self.assertTrue(result)
 
-    async def test_should_delete_file_when_queue_is_empty(self):
+    async def test_join_return_when_queue_is_empty(self):
         # given
         q = await Queue.create(self.data_path)
-        await q.put_nowait(ItemFactory)
-        # when
-        await q.get()
-        # then
-        self.assertFalse(self.data_path.exists())
+        # when/then
+        await q.join()
 
-    async def test_should_raise_error_when_calling_task_done_too_often(self):
+
+class TestInformationAboutQueue(QueueAsyncioTestCase):
+    async def test_should_report_as_empty(self):
         # given
         q = await Queue.create(self.data_path)
-        await q.put_nowait(ItemFactory)
-        await q.get()
-        await q.task_done()
         # when/then
-        with self.assertRaises(ValueError):
-            await q.task_done()
+        self.assertTrue(q.empty())
 
-    async def test_join_return_when_queue_is_empty(self):
+    async def test_should_not_report_as_empty(self):
         # given
         q = await Queue.create(self.data_path)
+        await q.put_nowait(ItemFactory())
         # when/then
-        await q.join()
-
-    async def test_should_raise_error_when_putting_into_full_queue(self):
-        # given
-        q = await Queue.create(self.data_path, maxsize=1)
-        await q.put_nowait(ItemFactory)
-        # when
-        with self.assertRaises(QueueFull):
-            await q.put_nowait(ItemFactory)
-
-    async def test_should_block_until_queue_has_free_slots(self):
-        async def producer(item):
-            await q.put(item)
-
-        async def consumer():
-            return await q.get()
-
-        # given
-        q = await Queue.create(self.data_path, maxsize=1)
-        await q.put_nowait("item-1")
-
-        # when
-        producer_task = asyncio.create_task(producer("item-2"))
-        await asyncio.sleep(1)  # producer sees a full queue when task starts
-        consumer_task = asyncio.create_task(consumer())
-        await asyncio.gather(producer_task, consumer_task)
-
-        item = await q.get_nowait()
-        # then
-        self.assertEqual(item, "item-2")
+        self.assertFalse(q.empty())
 
     async def test_full_should_return_true_when_queue_is_full(self):
         # given
         q = await Queue.create(self.data_path, maxsize=1)
         await q.put_nowait(ItemFactory)
         # when/then
         self.assertTrue(q.full())
@@ -194,13 +201,7 @@
         self.assertFalse(q.full())
 
     async def test_full_should_return_false_when_queue_is_not_limited(self):
         # given
         q = await Queue.create(self.data_path)
         # when/then
         self.assertFalse(q.full())
-
-    async def test_creating_queue_with_maxsize_below_0_yields_unlimited_queue(self):
-        # when
-        q = await Queue.create(self.data_path, maxsize=-1)
-        # then
-        self.assertEqual(q.maxsize, 0)
```

### Comparing `aiodiskqueue-0.1.0a8/PKG-INFO` & `aiodiskqueue-0.1.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

