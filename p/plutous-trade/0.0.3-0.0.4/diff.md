# Comparing `tmp/plutous_trade-0.0.3.tar.gz` & `tmp/plutous_trade-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous_trade-0.0.3.tar", max compression
+gzip compressed data, was "plutous_trade-0.0.4.tar", max compression
```

## Comparing `plutous_trade-0.0.3.tar` & `plutous_trade-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.3/LICENSE
--rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.3/README.md
--rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.3/plutous/__init__.py
--rw-r--r--   0        0        0       83 2023-05-23 08:28:34.235210 plutous_trade-0.0.3/plutous/trade/__init__.py
--rw-r--r--   0        0        0     3380 2023-05-23 04:04:54.046424 plutous_trade-0.0.3/plutous/trade/alembic.ini
--rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.3/plutous/trade/app/__init__.py
--rw-r--r--   0        0        0     1396 2023-05-23 08:28:17.690022 plutous_trade-0.0.3/plutous/trade/app/main.py
--rw-r--r--   0        0        0      590 2023-05-22 16:03:14.229359 plutous_trade-0.0.3/plutous/trade/app/models.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.3/plutous/trade/cli/__init__.py
--rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.3/plutous/trade/cli/database.py
--rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.3/plutous/trade/cli/main.py
--rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.3/plutous/trade/enums/__init__.py
--rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.3/plutous/trade/enums/action.py
--rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.3/plutous/trade/enums/asset_type.py
--rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.3/plutous/trade/enums/bot_type.py
--rw-r--r--   0        0        0       87 2023-05-16 18:50:39.068724 plutous_trade-0.0.3/plutous/trade/enums/position_side.py
--rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.3/plutous/trade/enums/strategy_direction.py
--rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.3/plutous/trade/enums/strategy_type.py
--rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.3/plutous/trade/migrations/README
--rw-r--r--   0        0        0     2275 2023-05-22 13:26:57.883694 plutous_trade-0.0.3/plutous/trade/migrations/env.py
--rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.3/plutous/trade/migrations/script.py.mako
--rw-r--r--   0        0        0     7883 2023-05-23 04:01:52.039288 plutous_trade-0.0.3/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py
--rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.3/plutous/trade/models/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.3/plutous/trade/models/api_key.py
--rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.3/plutous/trade/models/base.py
--rw-r--r--   0        0        0      977 2023-05-22 13:31:52.932067 plutous_trade-0.0.3/plutous/trade/models/bot.py
--rw-r--r--   0        0        0      941 2023-05-22 19:13:23.674596 plutous_trade-0.0.3/plutous/trade/models/position.py
--rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.3/plutous/trade/models/strategy.py
--rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.3/plutous/trade/models/trade.py
--rw-r--r--   0        0        0      560 2023-05-23 08:28:28.238780 plutous_trade-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.4/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.4/README.md
+-rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.4/plutous/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-28 12:54:48.055674 plutous_trade-0.0.4/plutous/trade/__init__.py
+-rw-r--r--   0        0        0     3380 2023-05-23 04:04:54.046424 plutous_trade-0.0.4/plutous/trade/alembic.ini
+-rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.4/plutous/trade/app/__init__.py
+-rw-r--r--   0        0        0     1396 2023-05-23 08:28:17.690022 plutous_trade-0.0.4/plutous/trade/app/main.py
+-rw-r--r--   0        0        0      616 2023-05-28 12:53:16.136715 plutous_trade-0.0.4/plutous/trade/app/models.py
+-rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.4/plutous/trade/cli/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.4/plutous/trade/cli/database.py
+-rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.4/plutous/trade/cli/main.py
+-rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.4/plutous/trade/enums/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.4/plutous/trade/enums/action.py
+-rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.4/plutous/trade/enums/asset_type.py
+-rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.4/plutous/trade/enums/bot_type.py
+-rw-r--r--   0        0        0       87 2023-05-16 18:50:39.068724 plutous_trade-0.0.4/plutous/trade/enums/position_side.py
+-rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.4/plutous/trade/enums/strategy_direction.py
+-rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.4/plutous/trade/enums/strategy_type.py
+-rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.4/plutous/trade/migrations/README
+-rw-r--r--   0        0        0     2252 2023-05-27 03:28:54.379452 plutous_trade-0.0.4/plutous/trade/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.4/plutous/trade/migrations/script.py.mako
+-rw-r--r--   0        0        0     7944 2023-05-28 12:54:19.153486 plutous_trade-0.0.4/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py
+-rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.4/plutous/trade/models/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.4/plutous/trade/models/api_key.py
+-rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.4/plutous/trade/models/base.py
+-rw-r--r--   0        0        0     1007 2023-05-28 12:51:29.676654 plutous_trade-0.0.4/plutous/trade/models/bot.py
+-rw-r--r--   0        0        0      941 2023-05-22 19:13:23.674596 plutous_trade-0.0.4/plutous/trade/models/position.py
+-rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.4/plutous/trade/models/strategy.py
+-rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.4/plutous/trade/models/trade.py
+-rw-r--r--   0        0        0      560 2023-05-28 12:54:52.496010 plutous_trade-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.4/PKG-INFO
```

### Comparing `plutous_trade-0.0.3/LICENSE` & `plutous_trade-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/alembic.ini` & `plutous_trade-0.0.4/plutous/trade/alembic.ini`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/app/main.py` & `plutous_trade-0.0.4/plutous/trade/app/main.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/app/models.py` & `plutous_trade-0.0.4/plutous/trade/app/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class BotPost(BaseModel):
     name: str
     strategy_id: int
     api_key_id: int
     type: BotType
     allocated_capital: float
     accumulate: bool = True
+    max_position: int = 1
 
 
 class ApiKeyPost(BaseModel):
     name: str
     exchange: Exchange
     key: str
     secret: str
```

### Comparing `plutous_trade-0.0.3/plutous/trade/cli/database.py` & `plutous_trade-0.0.4/plutous/trade/cli/database.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/enums/asset_type.py` & `plutous_trade-0.0.4/plutous/trade/enums/asset_type.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/migrations/env.py` & `plutous_trade-0.0.4/plutous/trade/migrations/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from logging.config import fileConfig
 
-from sqlalchemy import engine_from_config
-from sqlalchemy import pool, text
+from alembic import context
+from sqlalchemy import engine_from_config, pool, text
 
 from plutous.trade.models import Base
 
-from alembic import context
-
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
 # Interpret the config file for Python logging.
 # This line sets up loggers basically.
 if config.config_file_name is not None:
```

### Comparing `plutous_trade-0.0.3/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py` & `plutous_trade-0.0.4/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     op.create_index('ix_strategy_updated_at', 'strategy', ['updated_at'], unique=False, schema='trade')
     op.create_table('bot',
     sa.Column('name', sa.String(), nullable=False),
     sa.Column('type', sa.Enum('CUSTOM', 'WEBHOOK', name='bottype', schema='trade'), nullable=False),
     sa.Column('strategy_id', sa.Integer(), nullable=False),
     sa.Column('api_key_id', sa.Integer(), nullable=False),
     sa.Column('allocated_capital', sa.Float(), nullable=False),
+    sa.Column('max_position', sa.Integer(), nullable=False),
     sa.Column('accumulate', sa.Boolean(), nullable=False),
     sa.Column('id', sa.Integer(), nullable=False),
     sa.Column('created_at', sa.TIMESTAMP(), nullable=False),
     sa.Column('updated_at', sa.TIMESTAMP(), nullable=False),
     sa.ForeignKeyConstraint(['api_key_id'], ['trade.api_key.id'], ),
     sa.ForeignKeyConstraint(['strategy_id'], ['trade.strategy.id'], ),
     sa.PrimaryKeyConstraint('id'),
```

### Comparing `plutous_trade-0.0.3/plutous/trade/models/api_key.py` & `plutous_trade-0.0.4/plutous/trade/models/api_key.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/models/bot.py` & `plutous_trade-0.0.4/plutous/trade/models/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class Bot(Base):
     name: Mapped[str] = mapped_column(unique=True)
     type: Mapped[BotType] = mapped_column(Enum(BotType))
     strategy_id: Mapped[int] = mapped_column(ForeignKey(Strategy.id))
     api_key_id: Mapped[int] = mapped_column(ForeignKey(ApiKey.id))
     allocated_capital: Mapped[float]
+    max_position: Mapped[int]
     accumulate: Mapped[bool]
 
     api_key: Mapped[ApiKey] = relationship(ApiKey, back_populates="bots")
     strategy: Mapped[Strategy] = relationship(Strategy, back_populates="bots")
     positions: Mapped[list["Position"]] = relationship(
         "Position", back_populates="bot"
     )
```

### Comparing `plutous_trade-0.0.3/plutous/trade/models/position.py` & `plutous_trade-0.0.4/plutous/trade/models/position.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/models/strategy.py` & `plutous_trade-0.0.4/plutous/trade/models/strategy.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/plutous/trade/models/trade.py` & `plutous_trade-0.0.4/plutous/trade/models/trade.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.3/pyproject.toml` & `plutous_trade-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous-trade"
-version = "0.0.3"
+version = "0.0.4"
 description = "Plutous Trading Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous_trade-0.0.3/PKG-INFO` & `plutous_trade-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous-trade
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plutous Trading Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

