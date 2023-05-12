# Comparing `tmp/rum_with_telegram-0.9.9.tar.gz` & `tmp/rum_with_telegram-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.9.9.tar", last modified: Thu May 11 05:50:20 2023, max compression
+gzip compressed data, was "rum_with_telegram-1.0.0.tar", last modified: Thu May 11 12:13:41 2023, max compression
```

## Comparing `rum_with_telegram-0.9.9.tar` & `rum_with_telegram-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 05:50:20.006198 rum_with_telegram-0.9.9/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.9/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-11 05:50:20.005199 rum_with_telegram-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.9.9/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.9.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-11 05:50:19.944361 rum_with_telegram-0.9.9/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-11 05:49:31.000000 rum_with_telegram-0.9.9/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-0.9.9/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    25891 2023-05-11 05:49:36.000000 rum_with_telegram-0.9.9/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3479 2023-05-11 05:48:50.000000 rum_with_telegram-0.9.9/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1850 2023-05-04 04:25:42.000000 rum_with_telegram-0.9.9/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-11 05:50:20.002206 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-11 05:50:19.000000 rum_with_telegram-0.9.9/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 05:50:20.006198 rum_with_telegram-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-11 05:49:31.000000 rum_with_telegram-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:13:41.943184 rum_with_telegram-1.0.0/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-11 12:13:41.942188 rum_with_telegram-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.0/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-11 12:13:41.925240 rum_with_telegram-1.0.0/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-11 11:59:35.000000 rum_with_telegram-1.0.0/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-04 04:53:43.000000 rum_with_telegram-1.0.0/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    25411 2023-05-11 11:59:04.000000 rum_with_telegram-1.0.0/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3508 2023-05-11 12:00:11.000000 rum_with_telegram-1.0.0/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1900 2023-05-11 05:58:54.000000 rum_with_telegram-1.0.0/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-11 12:13:41.939222 rum_with_telegram-1.0.0/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-11 12:13:41.000000 rum_with_telegram-1.0.0/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-11 12:13:41.000000 rum_with_telegram-1.0.0/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 12:13:41.000000 rum_with_telegram-1.0.0/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-11 12:13:41.000000 rum_with_telegram-1.0.0/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-11 12:13:41.000000 rum_with_telegram-1.0.0/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 12:13:41.943184 rum_with_telegram-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-11 11:59:35.000000 rum_with_telegram-1.0.0/setup.py
```

### Comparing `rum_with_telegram-0.9.9/LICENSE` & `rum_with_telegram-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.9/PKG-INFO` & `rum_with_telegram-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.9.9
+Version: 1.0.0
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.9/rum_with_telegram/config.py` & `rum_with_telegram-1.0.0/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.9.9/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-1.0.0/rum_with_telegram/data_exchanger.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,55 +276,58 @@
         # channel post to rum group chain
         if update.channel_post:
             await self._handle_channel_post(update, context)
             return
         message = update.message or update.edited_message
         logger.info("handle_channel_message %s", message.message_id)
         channel_message_id = message.forward_from_message_id
-        chat_message_id = message.message_id
 
+        rum_post_url = None
         # send reply to user in group chat
-        for i in range(5):
+        for i in range(50):
             obj = self.db.get_trx_sent(channel_message_id)
             if not obj:
-                await asyncio.sleep(0.5)
+                await asyncio.sleep(0.1)
                 continue
             rum_post_url = obj.rum_post_url
             if not rum_post_url:
-                await asyncio.sleep(0.5)
+                await asyncio.sleep(0.1)
             else:
                 break
         if not rum_post_url:
             logger.warning("%s not found channel_message_id %s", i, channel_message_id)
-            return
-        logger.info("found rum_post_url %s", rum_post_url)
+        else:
+            logger.info("found rum_post_url %s", rum_post_url)
         await self._comment_with_feedurl(
-            context, "", message.chat.id, chat_message_id, rum_post_url
+            context, "", message.chat.id, message.message_id, rum_post_url
         )
         payload = {
-            "chat_message_id": chat_message_id,
+            "chat_message_id": message.message_id,
             "chat_type": message.chat.type,
             "channel_message_id": channel_message_id,
         }
         self.db.add_or_update(Relation, payload, "chat_message_id")
 
     async def _handle_reply_message(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         logger.info("start handle_reply_message %s", update.message.message_id)
-        username = update.message.from_user.username
-        userid = update.message.from_user.id
-        reply_msg = update.message.reply_to_message
+        message = update.message or update.edited_message
+        username = message.from_user.username
+        userid = message.from_user.id
+        reply_msg = message.reply_to_message
         channel_message_id = reply_msg.forward_from_message_id
         reply_chat_message_id = reply_msg.message_id
         reply_id = None
 
-        if channel_message_id:  # 直接回复 channel post
+        # comment to channel post
+        if channel_message_id:
             obj = self.db.get_trx_sent(channel_message_id)
             reply_id = obj.rum_post_id if obj else None
             logger.info("reply %s to channel_message_id %s", reply_id, channel_message_id)
-        elif reply_chat_message_id:  # 对回复的回复
+        # comment to reply
+        elif reply_chat_message_id:
             obj = self.db.get_first(
                 Relation,
                 {"chat_message_id": reply_chat_message_id, "trx_type": "comment"},
                 "chat_message_id",
             )
             if obj:
                 reply_id = obj.rum_post_id
@@ -336,78 +339,70 @@
                     channel_message_id,
                 )
                 if reply_id is None and channel_message_id:
                     obj = self.db.get_trx_sent(channel_message_id)
                     reply_id = obj.rum_post_id
                     logger.info("reply_id reset %s", reply_id)
 
-        if reply_id is None:
-            bot = Bot(token=context.bot.token)
-            _pinned = await bot.get_chat(self.config.TG_GROUP_ID)
-            _pinned = _pinned.pinned_message
-            channel_message_id = _pinned.forward_from_message_id
-            logger.info("get channel_message_id from pinned %s", channel_message_id)
-            reply_id = self.db.get_trx_sent(channel_message_id).rum_post_id
-            logger.info("channel_message_id to reply_id %s", reply_id)
-
         relation = await self.send_to_rum(
             context,
-            update.message,
+            message,
             userid,
             username,
             reply_id,
             channel_message_id,
         )
         relation.update(
             {
-                "chat_message_id": update.message.message_id,
-                "chat_type": update.message.chat.type,
+                "chat_message_id": message.message_id,
+                "chat_type": message.chat.type,
                 "channel_message_id": channel_message_id,
             }
         )
         self.db.add_or_update(Relation, relation, "trx_id")
 
     async def handle_group_message(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """handle group message"""
-        userid = update.message.from_user.id
+        message = update.message or update.edited_message
+        userid = message.from_user.id
         if userid in self.config.BLACK_LIST_TGIDS:
-            await update.message.reply_text("You are in the blacklist.")
+            await message.reply_text("You are in the blacklist.")
             return
 
-        if update.message.reply_to_message:
+        if message.reply_to_message:
             await self._handle_reply_message(update, context)
             return
         logger.info(
             "handle_group_message %s without reply_to_message",
-            update.message.message_id,
+            message.message_id,
         )
-        username = update.message.from_user.username
-        userid = update.message.from_user.id
+        username = message.from_user.username
+        userid = message.from_user.id
         bot = Bot(token=context.bot.token)
         _pinned = await bot.get_chat(self.config.TG_GROUP_ID)
         _pinned = _pinned.pinned_message
         channel_message_id = _pinned.forward_from_message_id
         obj = self.db.get_trx_sent(channel_message_id)
         if obj:
             reply_id = obj.rum_post_id
         else:
             reply_id = None
 
         relation = await self.send_to_rum(
             context,
-            update.message,
+            message,
             userid,
             username,
             reply_id,
             channel_message_id,
         )
         relation.update(
             {
-                "chat_message_id": update.message.message_id,
-                "chat_type": update.message.chat.type,
+                "chat_message_id": message.message_id,
+                "chat_type": message.chat.type,
                 "channel_message_id": channel_message_id,
             }
         )
         self.db.add_or_update(Relation, relation, "trx_id")
 
     async def command_start(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
         """/start command handler"""
```

### Comparing `rum_with_telegram-0.9.9/rum_with_telegram/db_handle.py` & `rum_with_telegram-1.0.0/rum_with_telegram/db_handle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from quorum_mininode_py import RumAccount
-from sqlalchemy import create_engine, not_
+from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.sql import func
 
 from rum_with_telegram.module import Base, Relation, UsedKey, User
 
 logger = logging.getLogger(__name__)
 
@@ -42,34 +42,33 @@
     def get_first_user(self, userid):
         return self.get_first(User, {"user_id": userid}, "user_id")
 
     def get_all(self, table, payload: dict, pk: str):
         with self.Session() as session:
             return session.query(table).filter_by(**{pk: payload[pk]}).all()
 
-    def get_trx_sent(self, channel_message_id):
+    def get_trx_sent_by(self, channel_message_id, chat_type):
         with self.Session() as session:
             relations = (
                 session.query(Relation)
-                .filter_by(channel_message_id=channel_message_id)
-                .filter(not_(chat_type="supergroup"))
+                .filter_by(channel_message_id=channel_message_id, chat_type=chat_type)
                 .all()
             )
             for relation in relations:
-                if relation.trx_id:
+                if relation and relation.trx_id:
                     return relation
-            relations = (
-                session.query(Relation)
-                .filter_by(channel_message_id=channel_message_id, chat_type="supergroup")
-                .all()
-            )
-            for relation in relations:
-                if relation.trx_id:
-                    return relation
-        return None
+            return None
+
+    def get_trx_sent(self, channel_message_id):
+        relation = self.get_trx_sent_by(channel_message_id, None)
+        if not relation:
+            relation = self.get_trx_sent_by(channel_message_id, "private")
+        if not relation:
+            relation = self.get_trx_sent_by(channel_message_id, "supergroup")
+        return relation
 
     def is_exist(self, table, payload: dict, pk: str):
         with self.Session() as session:
             return session.query(table).filter_by(**{pk: payload[pk]}).count() > 0
 
     def add_or_update(self, table, payload, pk):
         with self.Session() as session:
```

### Comparing `rum_with_telegram-0.9.9/rum_with_telegram/module.py` & `rum_with_telegram-1.0.0/rum_with_telegram/module.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from sqlalchemy import Column, DateTime, Integer, String, UniqueConstraint
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.sql import func
-
-Base = declarative_base()
-
-
-class Relation(Base):
-    """the map between trx and messages"""
-
-    __tablename__ = "relations"
-
-    id = Column(Integer, primary_key=True)
-    group_id = Column(String, default=None)
-    trx_id = Column(String, unique=True, index=True, default=None)
-    trx_type = Column(String, default=None)  # rum
-    rum_post_id = Column(String, default=None)  # rum
-    rum_post_url = Column(String, default=None)
-    chat_type = Column(String, default=None)
-    chat_message_id = Column(Integer, index=True, default=None)
-    channel_message_id = Column(Integer, index=True, default=None)
-    user_id = Column(String, default=None)  # telegram user id
-    pubkey = Column(String, default=None)  # rum group pubkey
-    created_at = Column(DateTime, default=func.now())
-    updated_at = Column(DateTime, onupdate=func.now())
-    __table_args__ = (
-        UniqueConstraint("group_id", "trx_id"),
-        UniqueConstraint("chat_type", "chat_message_id"),
-    )
-
-
-class User(Base):
-    __tablename__ = "users"
-
-    id = Column(Integer, primary_key=True)
-    user_id = Column(Integer, unique=True, index=True, default=None)
-    username = Column(String, index=True, default=None)
-    pvtkey = Column(String, unique=True, default=None)
-    pubkey = Column(String, unique=True, default=None)
-    address = Column(String, unique=True, default=None)
-    export_at = Column(DateTime, default=None)
-    created_at = Column(DateTime, default=func.now())
-    updated_at = Column(DateTime, onupdate=func.now())
-
-
-class UsedKey(Base):
-    __tablename__ = "used_keys"
-    id = Column(Integer, primary_key=True)
-    user_id = Column(Integer, index=True)
-    pvtkey = Column(String)
+from sqlalchemy import Column, DateTime, Integer, String, UniqueConstraint
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.sql import func
+
+Base = declarative_base()
+
+
+class Relation(Base):
+    """the map between trx and messages"""
+
+    __tablename__ = "relations"
+
+    id = Column(Integer, primary_key=True)
+    group_id = Column(String, default=None)
+    trx_id = Column(String, unique=True, index=True, default=None)
+    trx_type = Column(String, default=None)  # rum
+    rum_post_id = Column(String, default=None)  # rum
+    rum_post_url = Column(String, default=None)
+    chat_type = Column(String, default=None)
+    chat_message_id = Column(Integer, index=True, default=None)
+    channel_message_id = Column(Integer, index=True, default=None)
+    user_id = Column(String, default=None)  # telegram user id
+    pubkey = Column(String, default=None)  # rum group pubkey
+    created_at = Column(DateTime, default=func.now())
+    updated_at = Column(DateTime, onupdate=func.now())
+    __table_args__ = (
+        UniqueConstraint("group_id", "trx_id"),
+        UniqueConstraint("chat_type", "chat_message_id"),
+    )
+
+
+class User(Base):
+    __tablename__ = "users"
+
+    id = Column(Integer, primary_key=True)
+    user_id = Column(Integer, unique=True, index=True, default=None)
+    username = Column(String, index=True, default=None)
+    pvtkey = Column(String, unique=True, default=None)
+    pubkey = Column(String, unique=True, default=None)
+    address = Column(String, unique=True, default=None)
+    export_at = Column(DateTime, default=None)
+    created_at = Column(DateTime, default=func.now())
+    updated_at = Column(DateTime, onupdate=func.now())
+
+
+class UsedKey(Base):
+    __tablename__ = "used_keys"
+    id = Column(Integer, primary_key=True)
+    user_id = Column(Integer, index=True)
+    pvtkey = Column(String)
```

### Comparing `rum_with_telegram-0.9.9/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-1.0.0/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.9.9
+Version: 1.0.0
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.9.9/setup.py` & `rum_with_telegram-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.9.9",
+    version="1.0.0",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

