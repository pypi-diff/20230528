# Comparing `tmp/spothinta_api-0.2.0.tar.gz` & `tmp/spothinta_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spothinta_api-0.2.0.tar", max compression
+gzip compressed data, was "spothinta_api-0.3.0.tar", max compression
```

## Comparing `spothinta_api-0.2.0.tar` & `spothinta_api-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/LICENSE
--rw-r--r--   0        0        0     5127 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/README.md
--rw-r--r--   0        0        0     3607 2023-05-24 19:13:58.675229 spothinta_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      346 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/spothinta_api/__init__.py
--rw-r--r--   0        0        0      399 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/spothinta_api/const.py
--rw-r--r--   0        0        0      303 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/spothinta_api/exceptions.py
--rw-r--r--   0        0        0     5844 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/spothinta_api/models.py
--rw-r--r--   0        0        0        0 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/spothinta_api/py.typed
--rw-r--r--   0        0        0     4348 2023-05-24 19:13:35.945395 spothinta_api-0.2.0/spothinta_api/spothinta.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 spothinta_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5127 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/README.md
+-rw-r--r--   0        0        0     3607 2023-05-28 18:22:08.980031 spothinta_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/const.py
+-rw-r--r--   0        0        0      410 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/exceptions.py
+-rw-r--r--   0        0        0     6615 2023-05-28 18:21:41.739913 spothinta_api-0.3.0/spothinta_api/models.py
+-rw-r--r--   0        0        0        0 2023-05-28 18:21:41.743913 spothinta_api-0.3.0/spothinta_api/py.typed
+-rw-r--r--   0        0        0     4751 2023-05-28 18:21:41.743913 spothinta_api-0.3.0/spothinta_api/spothinta.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 spothinta_api-0.3.0/PKG-INFO
```

### Comparing `spothinta_api-0.2.0/LICENSE` & `spothinta_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spothinta_api-0.2.0/README.md` & `spothinta_api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spothinta_api-0.2.0/pyproject.toml` & `spothinta_api-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spothinta-api"
-version = "0.2.0"
+version = "0.3.0"
 description = "Asynchronous Python client providing energy prices from spot-hinta.fi"
 authors = ["Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>"]
 maintainers = ["Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["energy", "spothinta", "prices", "api", "async", "client"]
 classifiers = [
@@ -27,15 +27,15 @@
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.268"
+ruff = ">=0.0.243,<0.0.271"
 aresponses = "^2.1.6"
 black = "^22.12"
 blacken-docs = "^1.13.0"
 codespell = "^2.2.2"
 coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
 mypy = ">=1.0,<1.4"
 pre-commit = "^3.3.2"
```

### Comparing `spothinta_api-0.2.0/spothinta_api/models.py` & `spothinta_api-0.3.0/spothinta_api/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,26 +28,29 @@
             value = round(price, 5)
     return value
 
 
 def _get_pricetime(
     prices: dict[datetime, float],
     func: Callable[[dict[datetime, float]], datetime],
-) -> datetime:
+) -> datetime | None:
     """Return the time of the price.
 
     Args:
     ----
         prices: A dictionary with market prices.
         func: A function to get the time.
 
     Returns:
     -------
-        The time of the price.
+        The time of the price or None if prices is None or empty.
     """
+    if prices is None or len(prices) == 0:
+        return None
+
     return func(prices, key=prices.get)  # type: ignore[call-arg]
 
 
 @dataclass
 class Electricity:
     """Object representing electricity data."""
 
@@ -55,59 +58,80 @@
 
     @property
     def current_price(self) -> float | None:
         """Return the price for the current hour.
 
         Returns
         -------
-            The price for the current hour.
+            The price for the current hour or None if no price is available.
         """
         return self.price_at_time(self.utcnow())
 
     @property
-    def extreme_prices(self) -> tuple[float, float]:
-        """Return the minimum and maximum price.
+    def lowest_price_today(self) -> float | None:
+        """Return the minimum price today.
 
         Returns
         -------
-            The minimum and maximum price.
+            The minimum price today or None if no prices are available for today.
         """
-        return round(min(self.prices_today().values()), 5), round(
-            max(self.prices_today().values()),
-            5,
-        )
+        prices = self.prices_today()
+
+        if len(prices) == 0:
+            return None
+
+        return round(min(prices.values()), 5)
 
     @property
-    def average_price(self) -> float:
-        """Return the average price.
+    def highest_price_today(self) -> float | None:
+        """Return the maximum price today.
 
         Returns
         -------
-            The average price.
+            The maximum price today or None if no prices are available for today.
+        """
+        prices = self.prices_today()
+
+        if len(prices) == 0:
+            return None
+
+        return round(max(prices.values()), 5)
+
+    @property
+    def average_price(self) -> float | None:
+        """Return the average price today.
+
+        Returns
+        -------
+            The average price today or None if no prices are available for today.
         """
         prices_today = self.prices_today()
+
+        if len(prices_today) == 0:
+            return None
+
         return round(sum(prices_today.values()) / len(prices_today), 5)
 
     @property
-    def highest_price_time(self) -> datetime:
+    def highest_price_time(self) -> datetime | None:
         """Return the time of the highest price.
 
         Returns
         -------
-            The time of the highest price.
+            The time of the highest price or None if no prices are available for today.
         """
         return _get_pricetime(self.prices_today(), max)
 
     @property
-    def lowest_price_time(self) -> datetime:
+    def lowest_price_time(self) -> datetime | None:
         """Return the time of the lowest price.
 
         Returns
         -------
-            The time of the lowest price.
+            The time of the lowest price or None if no prices are available for today.
         """
         return _get_pricetime(self.prices_today(), min)
 
     @property
     def timestamp_prices(self) -> list[dict[str, float | datetime]]:
         """Return a dictionary with the prices.
```

### Comparing `spothinta_api-0.2.0/spothinta_api/spothinta.py` & `spothinta_api-0.3.0/spothinta_api/spothinta.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 import asyncio
 import socket
 from dataclasses import dataclass
 from importlib import metadata
 from typing import Any, cast
 
 import async_timeout
+from aiohttp import ClientResponseError
 from aiohttp.client import ClientError, ClientSession
 from aiohttp.hdrs import METH_GET
 from yarl import URL
 
 from .const import API_HOST, Region
-from .exceptions import SpotHintaConnectionError, SpotHintaError, SpotHintaNoDataError
+from .exceptions import (
+    SpotHintaConnectionError,
+    SpotHintaError,
+    SpotHintaNoDataError,
+    SpotHintaRateLimitError,
+)
 from .models import Electricity
 
 
 @dataclass
 class SpotHinta:
     """Main class for handling data fetching from spot-hinta.fi."""
 
@@ -42,14 +48,16 @@
 
         Returns:
         -------
             A Python dictionary (json) with the response from spot-hinta.fi.
 
         Raises:
         ------
+            SpotHintaRateLimitError: If too many requests have been made
+                during a given timespan.
             SpotHintaConnectionError: An error occurred while
                 communicating with the API.
             SpotHintaError: Received an unexpected response from
                 the API.
         """
         version = metadata.version(__package__)
 
@@ -74,24 +82,30 @@
                     method,
                     url,
                     params=params,
                     headers=headers,
                     ssl=True,
                 )
                 response.raise_for_status()
-        except asyncio.TimeoutError as exception:
+        except asyncio.TimeoutError as ex:
             msg = "Timeout occurred while connecting to the API."
             raise SpotHintaConnectionError(
                 msg,
-            ) from exception
-        except (ClientError, socket.gaierror) as exception:
+            ) from ex
+        except (ClientError, socket.gaierror) as ex:
+            if isinstance(ex, ClientResponseError) and ex.status == 429:
+                msg = "IP address rate limited (HTTP 429)"
+                raise SpotHintaRateLimitError(
+                    msg,
+                ) from ex
+
             msg = "Error occurred while communicating with the API."
             raise SpotHintaConnectionError(
                 msg,
-            ) from exception
+            ) from ex
 
         content_type = response.headers.get("Content-Type", "")
         if "application/json" not in content_type:
             text = await response.text()
             msg = "Unexpected content type response from the spot-hinta.fi API"
             raise SpotHintaError(
                 msg,
```

### Comparing `spothinta_api-0.2.0/PKG-INFO` & `spothinta_api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spothinta-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Asynchronous Python client providing energy prices from spot-hinta.fi
 License: MIT
 Keywords: energy,spothinta,prices,api,async,client
 Author: Sebastian Lövdahl
 Author-email: sebastian.lovdahl@hibox.fi
 Maintainer: Sebastian Lövdahl
 Maintainer-email: sebastian.lovdahl@hibox.fi
```

