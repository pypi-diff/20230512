# Comparing `tmp/pygame_cards-0.1.2.tar.gz` & `tmp/pygame_cards-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pygame_cards-0.1.3.tar", last modified: Fri May 12 13:04:01 2023, max compression
```

## Comparing `pygame_cards-0.1.2.tar` & `pygame_cards-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,49 @@
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/Makefile
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/api.rst
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/existing_sets.rst
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/make.bat
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/tutorial.rst
--rw-r--r--   0        0        0   141132 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/docs/images/emojis_52.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/README.md
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/classic_emojis_cards.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/first_game.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/minion_card.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/minion_card_graphics.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/minion_set.py
--rw-r--r--   0        0        0  1564010 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/images/DALL·E 2022-08-30 20.58.30 - frodo from lotr being obsessed with the ring, digital art.png
--rw-r--r--   0        0        0  1540208 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/images/DALL·E 2022-08-30 20.59.25 - gandalf from lotr looking very wise on his horse, digital art.png
--rw-r--r--   0        0        0  2099719 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/images/DALL·E 2022-08-30 21.01.56 - sam the hobbit from lotr sharing some elven bread, digital art.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/images/README.md
--rw-r--r--   0        0        0   446674 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/images/card_from_tuto.png
--rw-r--r--   0        0        0    29201 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/examples/tutorial/images/drawing_tuto.png
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/abstract.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/back.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/classics.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/deck.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/effects.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/events.py
--rw-r--r--   0        0        0    16746 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/hands.py
--rw-r--r--   0        0        0    10764 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/manager.py
--rw-r--r--   0        0        0     7155 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/set.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/utils.py
--rw-r--r--   0        0        0  1649238 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/images/DALL·E 2022-08-25 13.56.20 - funny happy python, digital art.png
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/images/readme.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/io/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/io/__main__.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/io/json.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pygame_cards/io/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pygame_cards-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.186595 pygame_cards-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 13:04:01.186595 pygame_cards-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.178595 pygame_cards-0.1.3/pygame_cards/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/classics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/deck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21155 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/hands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.182595 pygame_cards-0.1.3/pygame_cards/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1649238 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/images/DALL·E 2022-08-25 13.56.20 - funny happy python, digital art.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1649238 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/images/DEFAULT_CARDBACK.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.182595 pygame_cards-0.1.3/pygame_cards/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/io/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20690 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.186595 pygame_cards-0.1.3/pygame_cards/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/server/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/server/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/server/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/server/remote_players.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pygame_cards/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.178595 pygame_cards-0.1.3/pygame_cards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 13:04:01.000000 pygame_cards-0.1.3/pygame_cards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-12 13:04:01.000000 pygame_cards-0.1.3/pygame_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:04:01.000000 pygame_cards-0.1.3/pygame_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 13:04:01.000000 pygame_cards-0.1.3/pygame_cards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 13:04:01.000000 pygame_cards-0.1.3/pygame_cards.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:04:01.186595 pygame_cards-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:04:01.186595 pygame_cards-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/tests/test_cardset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-12 13:03:50.000000 pygame_cards-0.1.3/tests/test_events.py
```

### Comparing `pygame_cards-0.1.2/pygame_cards/abstract.py` & `pygame_cards-0.1.3/pygame_cards/abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
+from abc import abstractproperty
 from dataclasses import dataclass, field
 import logging
 import threading
 from typing import TYPE_CHECKING, Type
 import pygame
+from pygame_cards import constants
 
 
 if TYPE_CHECKING:
     from pygame_cards.set import CardsSet
 
 
 _CARDS_COUNTER = 0
@@ -19,43 +21,42 @@
     """The minimum required for a class.
 
     When inheriting from this class, use the decorator:
     @dataclass(eq=False)
     such that you can inherit from the hash method, which is safely
     handled by the u_id attribute.
 
-    :attr name: The name of the card
-    :attr u_id: A unique identifier for each card. Cards can be in
+    :param name: The name of the card
+    :param u_id: A unique identifier for each card. Cards can be in
         two similar exemplar, but will have different u_ids.
-    :attr graphics_type: The type of graphics we want to use.
+    :param graphics_type: The type of graphics we want to use.
+    :param logger: A :py:class:`logging.Logger` object.
+        Useful for debugging purposes.
+
     """
 
     name: str
 
     u_id: int = field(init=False)
     logger: logging.Logger = field(init=False, repr=False)
 
     graphics_type: Type[AbstractCardGraphics] = field(
         init=False,
         compare=False,
         repr=False,
     )
-    _graphics: AbstractCardGraphics = field(
-        init=False, compare=False, repr=False
-    )
+    _graphics: AbstractCardGraphics = field(init=False, compare=False, repr=False)
 
     def __post_init__(self):
         # Get a thread safe unique ID for that card
         with _COUNTER_LOCK:
             global _CARDS_COUNTER
             self.u_id = _CARDS_COUNTER
             _CARDS_COUNTER += 1
-        self.logger = logging.getLogger(
-            f"pywonders.cards.{type(self).__name__}"
-        )
+        self.logger = logging.getLogger(f"pywonders.cards.{type(self).__name__}")
 
     def __repr__(self) -> str:
         return f"Card({self.name})"
 
     def __hash__(self) -> int:
         return self.u_id
 
@@ -85,58 +86,97 @@
         test_set = [c for c in set if c.name == self.name]
         return len(test_set)
 
 
 class AbstractGraphic:
     """An abstract class for all the graphics used in the game.
 
-    :attr surface: The :py:class:`pygame.Surface`
-        corresponding to the current graphic.
+    The graphic is showed using the surface property, which is a pygame.Surface
+    object.
+    The size of the suface is also determined by the size property.
+    The suface should always be rendered for the desired size.
+    This helps showing cards well on screen with different sizes.
+
+    In case one need graphics of different sizes for the same object the best
+    is to create
+    two instances of graphics for the same object for performance reasons
+    (not having to recreate the surface every time).
+
+    :param surface: The :py:class:`pygame.Surface` corresponding to the current graphic.
+        This attribute must be implemented as a `cached property`.
+        Whe the size of the graphic is changed, the cached surface is
+        deleted and a new one is created.
+    :param size: The size of the graphic.
+        If you change that attribute, the surface will be recreated.
+    :param logger: The logger for this class. Useful for debugging.
 
     """
 
     surface: pygame.Surface
     logger: logging.Logger
+    size: tuple[int, int]
 
     def __init_subclass__(cls) -> None:
         # Assing a logger
-        cls.logger = logging.getLogger(f"pywonders.graphics.{cls.__name__}")
+        cls.logger = logging.getLogger(f"pygame_cards.graphics.{cls.__name__}")
 
     def clear_cache(self) -> None:
         """Clear the cache of this graphics.
 
         Usually you don't want to draw the same thing every time you
         will render a surface, so you will cache the surfaces.
         But sometimes the graphic will change and you will need to clear
         the cache of it.
         """
 
         # Remove the surface cache_property if exists
         self.__dict__.pop("surface", None)
 
+    @abstractproperty
+    def surface(self) -> pygame.Surface:
+        raise NotImplementedError(
+            f"'surface' is not implemented for {type(self).__name__}. Please use"
+            " the @cached_property decorator."
+        )
+
+    @property
+    def size(self) -> tuple[int, int]:
+        return self._size
+
+    @size.setter
+    def size(self, size: tuple[int, int]) -> None:
+        """Set the size of the graphic.
+
+        :param size: The size of the graphic.
+        """
+        if size == self._size:
+            return
+        self._size = size
+        self.clear_cache()
+
 
 @dataclass
 class AbstractCardGraphics(AbstractGraphic):
-    """A base representation for what the card should look like."""
+    """A base representation for what a card should look like."""
 
     card: AbstractCard
-    size: tuple[int, int] = 230, 350
+    size: tuple[int, int] = constants.CARD_SIZE
 
     @property
     def surface(self) -> pygame.Surface:
         """The surface of the card."""
 
         surf = pygame.Surface(self.size, pygame.SRCALPHA)
 
         rad = int(0.1 * min(*self.size))
         pygame.draw.rect(surf, "white", (0, 0, *self.size), 0, rad)
 
         return surf
 
 
 class Manager:
+    """Abstract class for cards manager."""
+
     logger: logging.Logger
 
     def __init__(self) -> None:
-        self.logger = logging.getLogger(
-            f"pygame_cards.manager.{type(self).__name__}"
-        )
+        self.logger = logging.getLogger(f"pygame_cards.manager.{type(self).__name__}")
```

### Comparing `pygame_cards-0.1.2/pygame_cards/back.py` & `pygame_cards-0.1.3/pygame_cards/back.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-from functools import cached_property
 import sys
-from time import sleep
+from functools import cached_property
+
 import pygame
-from pygame_cards.abstract import AbstractCard, AbstractCardGraphics
-from pygame_emojis import load_svg
 
+from pygame_cards.abstract import AbstractCard, AbstractCardGraphics
 from pygame_cards.utils import DEFAULT_CARDBACK
 
-CARD_BACK = AbstractCard("")
-
 
 class CardBackGraphics(AbstractCardGraphics):
-    """A simple graphics for a card back."""
+    """A simple graphics for a card back.
+
+    You can assign that graphics to any card you want.
+    """
 
     @cached_property
     def surface(self) -> pygame.Surface:
-        return pygame.transform.scale(
-            pygame.image.load(DEFAULT_CARDBACK), self.size
-        )
-
+        return pygame.transform.scale(pygame.image.load(DEFAULT_CARDBACK), self.size)
 
-CARD_BACK.graphics_type = CardBackGraphics
 
 if __name__ == "__main__":
+    from time import sleep
+
+    card_back = AbstractCard("")
+    card_back.graphics_type = CardBackGraphics
+    card_back.graphics.size = (300, 500)
     pygame.init()
 
     size = width, height = 1500, 700
 
     screen = pygame.display.set_mode(size)
     screen.fill("black")
 
-    position = (100 + CARD_BACK.graphics.size[0], 100)
+    position = (100 + card_back.graphics.size[0], 100)
 
     # Simply blit the card on the main surface
-    screen.blit(CARD_BACK.graphics.surface, position)
+    screen.blit(card_back.graphics.surface, position)
 
     while 1:
-
         for event in pygame.event.get():
-
             if event.type == pygame.QUIT:
                 sys.exit()
 
         pygame.display.flip()
 
         # Make sure you don't burn your cpu
         sleep(1)
```

### Comparing `pygame_cards-0.1.2/pygame_cards/classics.py` & `pygame_cards-0.1.3/pygame_cards/classics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-"""Classic games cards based on emojis.
+"""Classic playing cards module.
 
-This is based on emojis and cards are created at runtime.
+Many games use classic game cards.
+For that reason pygame_cards implements them using a simple api.
+
+
+The current implementation is based on emojis and graphics are created at runtime.
 """
 from __future__ import annotations
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from logging import warning
 import random
@@ -12,44 +16,50 @@
 import pygame
 from pygame_cards.abstract import AbstractCard
 from pygame_cards.abstract import AbstractCardGraphics
 from pygame_emojis import load_emoji, load_svg, find_code, _SVG_DIR
 
 from pygame_cards.effects import outer_halo, Decay
 from pygame_cards.set import CardsSet
+from pygame_cards.defaults import DefaultCardsSet
 
 
 class Colors(Enum):
+    """Colors of the cards."""
+
     SPADE = "♠"
     HEART = "♥"
     DIAMOND = "♦"
     CLUB = "♣"
 
 
 class Level(Enum):
+    """Levels of special cards."""
+
     JACK = "J"
     QUEEN = "Q"
     KING = "K"
     AS = "A"
 
 
+# Matching color strings
 RGBColor: dict[Colors, str] = {
     Colors.SPADE: "black",
     Colors.HEART: "red",
     Colors.DIAMOND: "red",
     Colors.CLUB: "black",
 }
-# Colors to specify an emoji version
+# Emoji color codes to specify an emoji version
 HEXEmojiColor: dict[Colors, str] = {
     Colors.SPADE: "1F3FB",
     Colors.HEART: "1F3FC",
     Colors.DIAMOND: "1F3FD",
     Colors.CLUB: "1F3FF",
 }
-
+# Emoji matching the levers
 LevelEmojis: dict[Level, str] = {
     Level.KING: "🤴",
     Level.QUEEN: "👸",
     Level.JACK: "💂",
 }
 
 
@@ -68,25 +78,19 @@
         self.__dict__.pop("symbols_rows", None)
         self.__dict__.pop("symbols_cols", None)
         self.__dict__.pop("top_label", None)
         self.__dict__.pop("icon_size", None)
 
     @cached_property
     def symbols_rows(self):
-        return [
-            self.size[1] / 8 * (i + 1) - self.icon_size[0] / 2
-            for i in range(7)
-        ]
+        return [self.size[1] / 8 * (i + 1) - self.icon_size[0] / 2 for i in range(7)]
 
     @cached_property
     def symbols_cols(self):
-        return [
-            self.size[0] / 4 * (i + 1) - self.icon_size[1] / 2
-            for i in range(3)
-        ]
+        return [self.size[0] / 4 * (i + 1) - self.icon_size[1] / 2 for i in range(3)]
 
     @cached_property
     def top_label(self) -> pygame.Surface:
         """The label at top of the cards."""
         scale = 0.15
         s = pygame.Surface(
             (int(self.size[0] * scale), int(self.size[1] * scale * 1.5)),
@@ -149,22 +153,19 @@
             (
                 self.size[0] - int(self.size[0] * scale_size),
                 self.size[1] - int(self.size[1] * scale_size) - y_offset,
             ),
         )
         # Add a face to the card
         if self.card.number in LevelEmojis:
-
             code_list = find_code(LevelEmojis[self.card.number])
             code = "-".join(code_list)
             emojis_files = [f for f in _SVG_DIR.rglob(f"{code}*.svg")]
             good_color = [
-                e
-                for e in emojis_files
-                if HEXEmojiColor[self.card.color] in e.stem
+                e for e in emojis_files if HEXEmojiColor[self.card.color] in e.stem
             ]
             # Dimension for the face
             w = self.size[0] * 0.8
             h = self.size[1] * 0.4
             face_surf = load_svg(good_color[0], size=(w, h))
             s.blit(
                 pygame.transform.flip(face_surf, False, True),
@@ -186,17 +187,15 @@
         elif isinstance(self.card.number, int):
             # place the icons
 
             icon_s = load_emoji(self.card.color.value, self.icon_size)
             flipped_icon = pygame.transform.flip(icon_s, False, True)
             r = self.symbols_rows
             c = self.symbols_cols
-            self.logger.debug(
-                f"{r=}, {c=}, {s.get_size()}, {icon_s.get_size()}"
-            )
+            self.logger.debug(f"{r=}, {c=}, {s.get_size()}, {icon_s.get_size()}")
             if self.card.number in [2, 3]:
                 s.blit(icon_s, (c[1], r[0]))
                 s.blit(flipped_icon, (c[1], r[-1]))
             if self.card.number > 3:
                 s.blit(icon_s, (c[0], r[0]))
                 s.blit(icon_s, (c[2], r[0]))
                 s.blit(flipped_icon, (c[0], r[-1]))
@@ -231,74 +230,98 @@
             warning(f"Could not decorate {self.card}")
 
         return s
 
 
 @dataclass(repr=False, eq=False)
 class NumberCard(AbstractCard):
-
     number: int | Level
     color: Colors
 
     graphics_type = EmojisFrenchSuits
 
+    def is_one_level_less_than(
+        self, other_card: NumberCard, as_equals_1: bool = False
+    ) -> bool:
+        """Return whether this card is one level less than the other_card.
+
+        :arg as_equals_1: Whether the As should be considered as 1 (worst of all)
+            or if it should be considered as the Best card
+        """
+        match other_card.number:
+            case Level.KING:
+                return self.number == Level.QUEEN
+            case Level.QUEEN:
+                return self.number == Level.JACK
+            case Level.JACK:
+                return self.number == 10
+            case Level.AS:
+                return False if as_equals_1 else self.number == Level.KING
+            case 2:
+                return self.number == Level.AS if as_equals_1 else False
+            case int():
+                if isinstance(self.number, Level):
+                    return False
+                return other_card.number == self.number + 1
+            case _:
+                raise NotImplementedError(f"{other_card.number = }")
+
 
 class CardSets:
     """Default card sets that can be used.
 
-    :attr n52: A 52 game cards.
-    :attr n36: A 36 game cards.
+    :param n52: A 52 game cards.
+    :param n36: A 36 game cards.
     """
 
     @classmethod
     @property
-    def n52(self) -> CardsSet[NumberCard]:
-        return CardsSet(
+    def n52(self) -> DefaultCardsSet[NumberCard]:
+        cardset = DefaultCardsSet(
             [
                 NumberCard(f"{n} of {c.value}", n, c)
                 for c in Colors
                 for n in [i for i in range(2, 11)] + [l for l in Level]
             ]
         )
+        cardset.name = "n52"
+        return cardset
 
     @classmethod
     @property
     def n36(self) -> CardsSet[NumberCard]:
-        return CardsSet(
+        cardset = DefaultCardsSet(
             [
                 NumberCard(f"{n} of {c.value}", n, c)
                 for c in Colors
                 for n in [i for i in range(6, 11)] + [l for l in Level]
             ]
         )
+        cardset.name = "n36"
+        return cardset
 
 
 if __name__ == "__main__":
-
     # This will visualize the cards
 
     pygame.init()
 
     size = width, height = 1500, 1000
 
     screen = pygame.display.set_mode(size)
 
     set = CardSets.n52
     counter = 0
     card = random.choice(set)
     print(set)
 
     # Add event to show the first card
-    pygame.event.post(
-        pygame.event.Event(pygame.KEYDOWN, {"key": pygame.K_LEFT})
-    )
+    pygame.event.post(pygame.event.Event(pygame.KEYDOWN, {"key": pygame.K_LEFT}))
     while 1:
-
         for event in pygame.event.get():
-
             if event.type == pygame.QUIT:
                 sys.exit()
 
             if event.type == pygame.KEYDOWN:
                 # Arrows allow to navigate around the cards
                 if event.key == pygame.K_LEFT:
                     counter -= 1
```

### Comparing `pygame_cards-0.1.2/pygame_cards/effects.py` & `pygame_cards-0.1.3/pygame_cards/effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Some effects for cards."""
 
 
 from enum import auto
 from math import sqrt
 import pygame
 
-from pywonders.cards.effect import AutoName
+from pygame_cards.utils import AutoName
 
 
 class Decay(AutoName):
     """Different decays for halos."""
 
     LINEAR = auto()
     QUADRATIC = auto()
@@ -84,51 +84,44 @@
             decay_func = lambda x: 1 - a * (min(x, radius) - radius) ** 2
         case Decay.NONE:
             decay_func = lambda x: 1
         case _:
             raise NotImplementedError(f"{decay = } not implemented.")
 
     halo_colors = [
-        inner_color.lerp(outer_color, decay_func(i))
-        for i in range(int(radius))
+        inner_color.lerp(outer_color, decay_func(i)) for i in range(int(radius))
     ]
     # A line surface to put the halo on
     line_surf = pygame.Surface((int(radius), 1), pygame.SRCALPHA)
     for i, c in enumerate(halo_colors):
         line_surf.set_at((i, 0), c)
 
     blit_right = [
         (line_surf, (inner_size[0] + radius, i))
         for i in range(radius, inner_size[1] + radius)
     ]
     surf.blits(blit_right)
 
     line_surf = pygame.transform.rotate(line_surf, 90)
-    blit_top = [
-        (line_surf, (i, 0)) for i in range(radius, inner_size[0] + radius)
-    ]
+    blit_top = [(line_surf, (i, 0)) for i in range(radius, inner_size[0] + radius)]
     surf.blits(blit_top)
 
     line_surf = pygame.transform.rotate(line_surf, 90)
-    blit_left = [
-        (line_surf, (0, i)) for i in range(radius, inner_size[1] + radius)
-    ]
+    blit_left = [(line_surf, (0, i)) for i in range(radius, inner_size[1] + radius)]
     surf.blits(blit_left)
 
     line_surf = pygame.transform.rotate(line_surf, 90)
     blit_bot = [
         (line_surf, (i, radius + inner_size[1]))
         for i in range(radius, inner_size[0] + radius)
     ]
     surf.blits(blit_bot)
 
     # Now do the same for the edge but it is 2D
-    coords = sum(
-        [[(i, j) for i in range(radius)] for j in range(radius)], start=[]
-    )
+    coords = sum([[(i, j) for i in range(radius)] for j in range(radius)], start=[])
     rads = [sqrt(i**2 + j**2) for i, j in coords]
     angle_surf = pygame.Surface((radius, radius), pygame.SRCALPHA)
     for coord, r in zip(coords, rads):
         angle_surf.set_at(coord, inner_color.lerp(outer_color, decay_func(r)))
     surf.blit(angle_surf, (inner_size[0] + radius, inner_size[1] + radius))
     angle_surf = pygame.transform.rotate(angle_surf, 90)
     surf.blit(angle_surf, (inner_size[0] + radius, 0))
```

### Comparing `pygame_cards-0.1.2/pygame_cards/hands.py` & `pygame_cards-0.1.3/pygame_cards/hands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,74 @@
-from abc import abstractmethod, abstractproperty
-from dataclasses import dataclass
 from enum import auto
 from functools import cached_property
 import logging
 from math import cos, sin, sqrt
 import math
-from time import sleep
+
 import pygame
+
 from pygame_cards.abstract import AbstractCard
 from pygame_cards.utils import AutoName
-from pygame_cards.abstract import AbstractGraphic
 from pygame_cards.effects import outer_halo
-from pygame_cards.set import CardsSet
+from pygame_cards.set import CardsSet, CardsetGraphic
+from pygame_cards import constants
 
 
 class CardOverlap(AutoName):
+    """How card overlap in the hand."""
+
     left = auto()
     right = auto()
 
 
-@dataclass
-class CardsetGraphic(AbstractGraphic):
-    """A base graphic fro any card holder.
-
-    :attr cardset: The set of card that is shown.
-    :attr size: A tuple with the size of the requested card in this graphic.
-    :attr card_size: A tuple with the size of the cards in this graphic.
-    :attr card_border_radius: The radius of the cards in this card set.
-    :attr max_cards: The max number of card that can be contained in this
-        graphic. If 0, this is unlimited.
-    """
-
-    cardset: CardsSet
-
-    # Defualt hand size
-    size: tuple[int, int] = (900, 240)
-    card_size: tuple[int, int] = (135, 200)
-    card_border_radius: int = 20
-
-    max_cards: int = 0
-
-    graphics_type: type | None = None
-
-    def __post_init__(self):
-
-        for card in self.cardset:
-            # Enforce the type
-            if self.graphics_type:
-                card.graphics_type = self.graphics_type
-            # Enforce the card size
-            card.graphics.size = self.card_size
-        self._raised_with_hovered_warning = False
-
-    @abstractproperty
-    def surface(self) -> pygame.Surface:
-        raise NotImplementedError(
-            f"property 'surface' in {type(self).__name__}"
-        )
-
-    @abstractmethod
-    def get_card_at(self, pos: tuple[int, int]) -> AbstractCard | None:
-        """Return the card at the given pixel position
-
-        :arg pos: The position inside the CardsetGraphic surface.
-        """
-        raise NotImplementedError(
-            f"'get_card_at' in Class {type(self).__name__}"
-        )
-
-    def remove_card(self, card: AbstractCard) -> None:
-        """Remove a card from the cardset."""
-
-        self.cardset.remove(card)
-        self.clear_cache()
-
-    def append_card(self, card: AbstractCard) -> None:
-        """Append a card to the cardset."""
-
-        self.cardset.append(card)
-        card.graphics.size = self.card_size
-        card.graphics.clear_cache()
-        self.clear_cache()
-
-    def with_hovered(self, card: AbstractCard | None) -> pygame.Surface:
-        """Show the hand with the card hovered."""
-        if not self._raised_with_hovered_warning:
-            logging.warning(
-                f"Not implemented `with_hovered()` in {type(self).__name__}",
-            )
-            self._raised_with_hovered_warning = True
-        return self.surface
-
-
-@dataclass
 class BaseHand(CardsetGraphic):
     """A base class for a hand.
 
     Usually in a hand the cards are shown on next to the other.
 
-    :attr overlap_hide: The card to hide if to cards are one
+    :param overlap_hide: The card to hide if to cards are one
         over each other. By default the card overlap on the right,
         which is the standard in card games.
         This also implies that the cards are located at the opposite side
         of their overlap.
 
 
     """
 
-    overlap_hide: CardOverlap = CardOverlap.right
+    def __init__(
+        self,
+        *args,
+        overlap_hide: CardOverlap = CardOverlap.right,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.overlap_hide = overlap_hide
 
 
-@dataclass
 class AlignedHand(BaseHand):
     """A hand of card with all the cards aligned.
 
-    :attr offset_position: The offset of the position between the cards.
+    :param card_spacing: The offset proportion of the position between the cards.
 
         * 0, means the cards are directly next to each other.
         * Positive offset, means the card will be further
             away from each other.
         * Negative, means cards will be closer
             to each other.
 
     """
 
-    offset_position: float = 20
+    def __init__(
+        self,
+        *args,
+        card_spacing: float = constants.COLUMN_SPACING,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.card_spacing = card_spacing
 
     @cached_property
     def surface(self) -> pygame.Surface:
         """The surface of the hand."""
         surf = pygame.Surface(self.size, pygame.SRCALPHA)
 
         x_positions, offset = self.calculate_x_positions()
@@ -154,54 +94,50 @@
 
         :return (x_positions, offset_value):
             The x_positions is the positions of each card.
             The offset_value is the value used to make the
             spacing between the cards.
         """
         # calculate dimenstions required for the displayed surf
-        offset = self.offset_position
+        offset = self.card_spacing * self.card_size[0]
         total_x = (
-            len(self.cardset) * self.card_size[0]
-            + (len(self.cardset) - 1) * offset
+            len(self.cardset) * self.card_size[0] + (len(self.cardset) - 1) * offset
         )
 
         if total_x > self.size[0]:
-            self.logger.warning(
-                "Too many cards for hands size, rescaling will apply."
-            )
+            self.logger.warning("Too many cards for hands size, rescaling will apply.")
             offset = (self.size[0] - len(self.cardset) * self.card_size[0]) / (
                 len(self.cardset) - 1
             )
         x_positions = [
-            i * self.card_size[0] + (i + 1) * offset
-            for i in range(len(self.cardset))
+            i * self.card_size[0] + i * offset for i in range(len(self.cardset))
         ]
         # Revert the position in case of another overlap
         x_positions = [
             x_pos
             if self.overlap_hide == CardOverlap.right
             else self.size[0] - self.card_size[0] - x_pos
             for x_pos in x_positions
         ]
+        self.logger.debug(f"{x_positions=}")
+
         return x_positions, offset
 
     def with_hovered(
         self, card: AbstractCard | None, radius: float = 20, **kwargs
     ) -> pygame.Surface:
         if card is None:
             return pygame.Surface((0, 0))
         index = self.cardset.index(card)
         self.logger.debug(f"{index=}")
         x_posistions, _ = self.calculate_x_positions()
         x_pos = x_posistions[index]
 
         card.graphics.size = self.card_size
-        highlighted_surf = outer_halo(
-            card.graphics.surface, radius=radius, **kwargs
-        )
+        highlighted_surf = outer_halo(card.graphics.surface, radius=radius, **kwargs)
         # assume the center will be on it
         out_surf = pygame.Surface(self.size, pygame.SRCALPHA)
         highlighted_surf = pygame.transform.scale(
             highlighted_surf,
             (self.card_size[0] + 2 * radius, self.card_size[1] + 2 * radius),
         )
         out_surf.blit(
@@ -211,74 +147,87 @@
         out_surf.blit(
             card.graphics.surface,
             (x_pos, self.calculate_y_position()),
         )
         return out_surf
 
     def get_card_at(self, pos: tuple[int, int]) -> AbstractCard | None:
-        """Return the card at the given pixel position
-
-        :arg pos: The position inside the CardsHand surface.
-        """
         s = self.surface.get_size()
         if not (pos[0] < s[0] and pos[1] < s[1]):
-            self.logger.error(f"get_card_at:{pos=} not in {s}.")
+            self.logger.error(f"get_card_at({pos=}) not in {s}.")
             return None
 
         x_positions, offset = self.calculate_x_positions()
-        self.logger.debug(f"get_card_at:{x_positions=}, {self.overlap_hide=}")
+        self.logger.debug(f"get_card_at({pos=}): {x_positions=}, {self.overlap_hide=}")
 
         # TODO: make this work
         for card_index, x_pos in enumerate(x_positions):
             if pos[0] < x_pos or pos[0] > x_pos + self.card_size[0]:
                 self.logger.debug(
-                    f"get_card_at: {card_index=} is not Between the card boundaries"
+                    f"get_card_at({pos=}):: {card_index=} is not Between the card"
+                    " boundaries"
                 )
                 continue
             if (
                 self.overlap_hide == CardOverlap.right
                 # Check that is not under the next card
-                and pos[0] - x_pos > self.card_size[0] + self.offset_position
+                and pos[0] - x_pos
+                > self.card_size[0] + self.card_spacing * self.card_size[0]
             ) or (
                 self.overlap_hide == CardOverlap.left
-                and pos[0] - x_pos < self.offset_position
+                and pos[0] - x_pos < self.card_spacing * self.card_size[0]
             ):
                 self.logger.debug(
-                    f"get_card_at: {card_index=} is  going to be under the next card"
+                    f"get_card_at({pos=}):: {card_index=} is  going to be under the"
+                    " next card"
                 )
                 continue
             if x_pos - pos[0] > self.card_size[0] + offset:
-                self.logger.debug(f"get_card_at:{pos=} is in offset.")
+                self.logger.debug(f"get_card_at({pos=}): is in offset.")
                 continue  # Between two cards, in the offset
 
-            self.logger.debug(f"get_card_at:{pos=} found index {card_index}.")
+            self.logger.debug(f"get_card_at({pos=}): found index {card_index}.")
             return self.cardset[card_index]
 
         return None
 
+    def get_card_positions(self) -> dict[AbstractCard, tuple[int, int]]:
+        y = self.calculate_y_position()
+        xs, _ = self.calculate_x_positions()
+
+        return {card: (x, y) for card, x in zip(self.cardset, xs)}
+
 
-@dataclass
 class RoundedHand(BaseHand):
     """A hand of card with all the cards aligned on an arc of a circle.
 
     This will produced an hand of card where cards are clipped insided
     the size of the hand.
 
 
-    :attr angle: The angle in which the cards are constrained
+    :param angle: The angle in which the cards are constrained
         (Unit: Degrees)
         If 0, the cards are all aligned.
         If not zero, the cards will be placed on an arc of a circle
         with the given angle.
 
     """
 
-    angle: float = 90
-    # Change the defualt size
-    size: tuple[float, float] = (700, 400)
+    def __init__(
+        self,
+        *args,
+        angle: float = 90,
+        **kwargs,
+    ):
+        if not "size" in kwargs:
+            # Change the defualt size
+            kwargs["size"] = (700, 400)
+
+        super().__init__(*args, **kwargs)
+        self.angle = angle
 
     def _max_card_h(self) -> float:
         """Return the maximum height that a card can do in surface."""
         return sqrt(
             self.card_size[0] * self.card_size[0]
             + self.card_size[1] * self.card_size[1]
         )
@@ -292,25 +241,22 @@
             # Special cases, show aligned
             angles = [0] * len(self.cardset)
         else:
             angle_step = self.angle / (len(self.cardset) - 1)
             self.logger.debug(f"{angle_step=}")
             # from the center, angle = 0, which is the central card and ref point.
             angles = [
-                -self.angle / 2 + i * angle_step
-                for i in range(len(self.cardset))
+                -self.angle / 2 + i * angle_step for i in range(len(self.cardset))
             ]
         # Radius of the circle around the cards (from center to card centers)
         # Trust me, I am an engineer
         card_diagonal = sqrt(self.card_size[0] ** 2 + self.card_size[1] ** 2)
         radius = min(
             # Constraint for width
-            (self.size[0] - card_diagonal)
-            / 2
-            / sin(math.radians(self.angle / 2)),
+            (self.size[0] - card_diagonal) / 2 / sin(math.radians(self.angle / 2)),
             # Constraint for heigth
             (self.size[1] - self.card_size[1] - card_diagonal / 2)
             / (1 - cos(math.radians(self.angle / 2))),
         )
         self.logger.debug(f"{radius = }")
         # TODO: correct the angle if the radius is smaller than a threshold
 
@@ -349,152 +295,341 @@
                 - card_surf.get_size()[1],
             )
             for a, card_surf in zip(angles, rotated_surfs)
         ]
         self.logger.debug(f"{card_positions=}")
 
         for card_surf, card_pos in zip(rotated_surfs, card_positions):
-
             surf.blit(
                 card_surf,
                 card_pos,
             )
 
         self._radius = radius
         self._center_pos = center_pos
         self._card_diagonal = card_diagonal
         self._angles = angles
 
         return surf
 
     def get_card_at(self, pos: tuple[int, int]) -> AbstractCard | None:
         # We think pos1 from bottom instead of top
-        if (
-            pos[0] < 0
-            or pos[1] < 0
-            or pos[0] > self.size[0]
-            or pos[1] > self.size[1]
-        ):
+        if pos[0] < 0 or pos[1] < 0 or pos[0] > self.size[0] or pos[1] > self.size[1]:
             self.logger.debug(f"{pos=} ut of bound")
             return None
 
         pos = (pos[0], self.size[1] - pos[1])
         self.logger.debug(f"Converted {pos=}")
         self.logger.debug(f"Center {self._center_pos=}")
 
         dist_to_center = sqrt(
-            (pos[0] - self._center_pos[0]) ** 2
-            + (pos[1] - self._center_pos[1]) ** 2
+            (pos[0] - self._center_pos[0]) ** 2 + (pos[1] - self._center_pos[1]) ** 2
         )
         self.logger.debug(f"{dist_to_center=}")
         if (
             dist_to_center > self._radius + self._card_diagonal / 2
             or dist_to_center < self._radius - self._card_diagonal / 2
         ):
             self.logger.debug(f"{pos=} is not in radius range")
             return None
 
         for card, angle in zip(reversed(self.cardset), reversed(self._angles)):
             # Reverse because cards at the end are over the previous
             self.logger.debug(f"Check {card=} with {angle=}")
             card_center = (
-                (
-                    self._center_pos[0]
-                    + sin(math.radians(angle)) * self._radius
-                ),
-                (
-                    self._center_pos[1]
-                    + cos(math.radians(angle)) * self._radius
-                ),
+                (self._center_pos[0] + sin(math.radians(angle)) * self._radius),
+                (self._center_pos[1] + cos(math.radians(angle)) * self._radius),
             )
             dist_to_card_center = sqrt(
                 (pos[0] - card_center[0]) ** 2 + (pos[1] - card_center[1]) ** 2
             )
             # Cosine theorem to find angle (center, card, pos)
             # {\displaystyle a^{2}=c^{2}+b^{2}-2bc\cos \alpha }.
             a = math.acos(
-                (
-                    dist_to_center**2
-                    - dist_to_card_center**2
-                    - self._radius**2
-                )
+                (dist_to_center**2 - dist_to_card_center**2 - self._radius**2)
                 / (-2 * dist_to_card_center * self._radius)
             )
             # Distance to the line from the center to the center of the card
             dist_to_line = sin(a) * dist_to_card_center
             self.logger.debug(f"Calculated {dist_to_line=}")
             if dist_to_line < self.card_size[0] / 2:
                 return card
         return None
 
+    def get_card_positions(self) -> dict[AbstractCard, tuple[int, int]]:
+        # use aligned hand as a proxy
+        self.card_spacing = constants.COLUMN_SPACING
+        y = AlignedHand.calculate_y_position(self)
+        xs, _ = AlignedHand.calculate_x_positions(self)
+
+        self.logger.warning(
+            f"'get_card_positions' is not perfectly correct implemented yet"
+        )
+
+        return {card: (x, y) for card, x in zip(self.cardset, xs)}
+
 
-@dataclass
-class PlayingHand(BaseHand):
-    """A representation of the hand of the player.
+class Pile(CardsetGraphic):
+    """A pile has only its last/s card/s that can be selected.
 
-    This will show the cards how the player wants it.
+    :param rel_offset: The offset between cards. Relative to the card size.
 
-    Currently only works with size and card_size being specified.
-    TODO: optimize by caching the variables.
     """
 
-    @abstractmethod
-    def hovered(self, card: AbstractCard) -> pygame.Surface:
-        """Show the hand with the card hovered."""
-
-    @abstractmethod
-    def with_going_to_play(self, card: AbstractCard) -> pygame.Surface:
-        """Show the hand with the card that is going to be played.
+    def __init__(
+        self,
+        *args,
+        rel_offset: float = 0.2,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.rel_offset = rel_offset
+
+    def _get_card_index_at(self, pos: tuple[int, int]) -> int | None:
+        """Return the index of the card located at the current position."""
+        raise NotImplementedError(f"Must implement in {type(self).__name__}")
+
+    def get_card_at(self, pos: tuple[int, int]) -> AbstractCard | None:
+        idx = self._get_card_index_at(pos)
+
+        return None if idx is None else self.cardset[idx]
+
+    def get_cards_at(self, pos: tuple[int, int]) -> CardsSet | None:
+        """Return the card set at the given pixel position
 
-        This can be used for asking a confimation to the user,
-        or for aking a way to play the card.
+        :arg pos: The position inside the CardsetGraphic surface.
         """
+        idx = self._get_card_index_at(pos)
 
+        return None if idx is None else self.cardset[idx:]
+
+
+class VerticalPileGraphic(Pile):
+    """Show a column in cards aligned.
+
+    Cards are shown from first one to the last one on the bottom.
+
+    """
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        if not "size" in kwargs:
+            # Change the defualt size
+            kwargs["size"] = (175, 400)
+
+        super().__init__(*args, **kwargs)
+
+    def clear_cache(self) -> None:
+        # Remove the surface cache_property if exists
+        self.__dict__.pop("y_positions", None)
+        super().clear_cache()
+
+    @property
+    def size(self) -> tuple[int, int]:
+        return super().size
+
+    @size.setter
+    def size(self, size: tuple[int, int]) -> None:
+        super(VerticalPileGraphic, VerticalPileGraphic).size.__set__(self, size)
+        # Cards are too large for the new pile size
+        if self.card_size[0] > self.size[0]:
+            width = self.size[0]
+            # Keep the same ratio
+            height = width / self.card_size[0] * self.card_size[1]
+
+            self.card_size = (width, height)
+            self.logger.debug(f"setting card size to {self.card_size=}")
+
+    @cached_property
+    def surface(self) -> pygame.Surface:
+        # Create the surface
+        surf = pygame.Surface(self.size, pygame.SRCALPHA)
+
+        # Calculate how we position the cards
+        n_cards = len(self.cardset)
+        if n_cards == 0:
+            return surf
+
+        self.logger.debug(f"{self.size=}, {self.card_size=}")
+
+        x_position = (self.size[0] - self.card_size[0]) / 2
+
+        # Add the cards on the surface
+        surf.blits(
+            [
+                (card.graphics.surface, (x_position, y))
+                for card, y in zip(self.cardset, self.y_positions)
+            ],
+        )
+
+        return surf
+
+    @cached_property
+    def y_positions(self) -> list[int]:
+        n_cards = len(self.cardset)
+        max_offset = self.rel_offset * self.card_size[1]
+
+        expected_h = n_cards * max_offset + self.card_size[1]
+        h_space = (
+            (self.size[1] - self.card_size[1]) / n_cards
+            if expected_h > self.size[1]
+            else max_offset
+        )
+        return [i * h_space for i in range(n_cards)]
+
+    def _get_card_index_at(self, pos: tuple[int, int]) -> int | None:
+        """Return the index of the card located at the current position."""
+        if not self.cardset:
+            # No cards case
+            return None
+        # Iterate over the cards and position to find the correct card
+
+        for card_idx in range(len(self.cardset)):
+            if pos[1] < self.y_positions[card_idx]:
+                return card_idx - 1
+        if pos[1] < self.y_positions[-1] + self.card_size[1]:
+            # Last card is on top
+            return len(self.cardset) - 1
+        return None
+
+    def get_card_positions(self) -> dict[AbstractCard, tuple[int, int]]:
+        x_position = (self.size[0] - self.card_size[0]) / 2
+
+        return {
+            card: (x_position, y) for card, y in zip(self.cardset, self.y_positions)
+        }
 
-if __name__ == "__main__":
 
+class HorizontalPileGraphic(Pile):
+    """Show a cards horizontally aligned.
+
+    Cards are shown from first one to the last one on the bottom.
+
+    """
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        if not "size" in kwargs:
+            # Change the defualt size
+            kwargs["size"] = (350, 240)
+
+        super().__init__(*args, **kwargs)
+
+    def clear_cache(self) -> None:
+        # Remove the surface cache_property if exists
+        self.__dict__.pop("x_positions", None)
+        super().clear_cache()
+
+    @cached_property
+    def surface(self) -> pygame.Surface:
+        # Create the surface
+        surf = pygame.Surface(self.size, pygame.SRCALPHA)
+
+        # Calculate how we position the cards
+        n_cards = len(self.cardset)
+        if n_cards == 0:
+            return surf
+
+        y_position = (self.size[1] - self.card_size[1]) / 2
+
+        # Add the cards on the surface
+        surf.blits(
+            [
+                (card.graphics.surface, (x, y_position))
+                for card, x in zip(self.cardset, self.x_positions)
+            ],
+        )
+
+        return surf
+
+    @cached_property
+    def x_positions(self) -> list[int]:
+        n_cards = len(self.cardset)
+        # Get the offset between cards in pixels
+        offset = self.rel_offset * self.card_size[0]
+
+        expected_h = n_cards * offset + self.card_size[0]
+        h_space = (
+            (self.size[0] - self.card_size[0]) / n_cards
+            if expected_h > self.size[0]
+            else offset
+        )
+        return [i * h_space for i in range(n_cards)]
+
+    def _get_card_index_at(self, pos: tuple[int, int]) -> int | None:
+        """Return the index of the card located at the current position."""
+        if not self.cardset:
+            # No cards case
+            return None
+        # Iterate over the cards and position to find the correct card
+
+        for card_idx in range(len(self.cardset)):
+            if pos[0] < self.x_positions[card_idx]:
+                return card_idx - 1
+        if pos[0] < self.x_positions[-1] + self.card_size[0]:
+            # Last card is on top
+            return len(self.cardset) - 1
+        return None
+
+    def get_card_positions(self) -> dict[AbstractCard, tuple[int, int]]:
+        y_position = (self.size[1] - self.card_size[1]) / 2
+
+        return {
+            card: (x, y_position) for card, x in zip(self.cardset, self.x_positions)
+        }
+
+
+if __name__ == "__main__":
     # This will visualize the cards
 
     import sys
     import pygame
     from pygame_cards.classics import CardSets as ClassicCardSet
 
     logging.basicConfig()
 
     pygame.init()
 
-    size = width, height = 1500, 700
+    size = width, height = 1500, 1200
 
     screen = pygame.display.set_mode(size)
 
     card_set = CardsSet(ClassicCardSet.n52[:4])
 
     graphics_aligned = AlignedHand(card_set)
-    graphics_aligned_overlap = AlignedHand(card_set, offset_position=-29)
+    graphics_aligned_overlap = AlignedHand(card_set, card_spacing=-0.15)
     graphics_rounded = RoundedHand(card_set + card_set + card_set)
     graphics_rounded2 = RoundedHand(card_set + card_set)
 
-    graphics_aligned.logger.setLevel(logging.DEBUG)
+    # graphics_aligned.logger.setLevel(logging.DEBUG)
     graphics_aligned_overlap.logger.setLevel(logging.DEBUG)
-    graphics_rounded.logger.setLevel(logging.DEBUG)
-    graphics_rounded2.logger.setLevel(logging.DEBUG)
+    # graphics_rounded.logger.setLevel(logging.DEBUG)
+    # graphics_rounded2.logger.setLevel(logging.DEBUG)
 
     screen.blit(graphics_aligned.surface, (200, 0))
     screen.blit(graphics_aligned_overlap.surface, (200, 200))
     screen.blit(graphics_rounded.surface, (200, 400))
     screen.blit(graphics_rounded2.surface, (200, 750))
 
     pygame.display.flip()
 
+    clock = pygame.time.Clock()
+    fps = 4
+
     while 1:
         pos = pygame.mouse.get_pos()
         hoverd_card = graphics_aligned.get_card_at((pos[0] - 200, pos[1] - 0))
         screen.blit(
-            graphics_aligned.with_hovered(hoverd_card, fill_inside=False),
+            graphics_aligned.with_hovered(hoverd_card, fill_inside=True),
             (200, 0),
         )
         pygame.display.update()
-        sleep(1)
+        clock.tick(fps)
         for event in pygame.event.get():
-
             if event.type == pygame.QUIT:
                 sys.exit()
```

### Comparing `pygame_cards-0.1.2/pygame_cards/utils.py` & `pygame_cards-0.1.3/pygame_cards/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from enum import Enum
 from pathlib import Path
 from pygame import Surface
 
 import pygame_cards
 
+from urllib.request import urlretrieve
+
 
 DEFAULT_CARDBACK = Path(
     *pygame_cards.__path__,
-    "images/DALL·E 2022-08-25 13.56.20 - funny happy python, digital art.png",
+    "images/DEFAULT_CARDBACK.png",
 )
+if not DEFAULT_CARDBACK.is_file():
+    DEFAULT_CARDBACK.parent.mkdir(parents=True, exist_ok=True)
+
+    urlretrieve(
+        "https://github.com/ScienceGamez/pygame_cards/raw/main/"
+        "pygame_cards/images/DEFAULT_CARDBACK.png",
+        DEFAULT_CARDBACK,
+    )
 
 
 class AutoName(Enum):
     def _generate_next_value_(name, start, count, last_values):
         return name
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygame_cards-0.1.2/pygame_cards/images/DALL·E 2022-08-25 13.56.20 - funny happy python, digital art.png` & `pygame_cards-0.1.3/pygame_cards/images/DALL·E 2022-08-25 13.56.20 - funny happy python, digital art.png`

 * *Files identical despite different names*

### Comparing `pygame_cards-0.1.2/pygame_cards/io/json.py` & `pygame_cards-0.1.3/pygame_cards/io/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,15 @@
         else cards_list.pop(0)
     )
 
     additional_cards_dicts = []
     for card_dict in cards_list:
         # Find at which number of player the card should be added
         if "add_card_at_playercount" in card_dict.keys():
-
-            player_counts: list[int] = card_dict.pop(
-                "add_card_at_playercount", [1]
-            )
+            player_counts: list[int] = card_dict.pop("add_card_at_playercount", [1])
             if isinstance(player_counts, list):
                 # Make a Mik mack to correctly add the cards
                 card_dict["add_card_at_playercount"] = player_counts[0]
                 for count in player_counts[1:]:
                     new_dict = card_dict.copy()
                     new_dict["add_card_at_playercount"] = count
                     additional_cards_dicts.append(new_dict)
@@ -67,21 +64,17 @@
     """
     if not isinstance(files, list):
         logging.getLogger("pygame_cards.from_jsons").debug(
             f"Received a single file {files}"
         )
         if isinstance(card_types, list):
             raise TypeError(
-                "Impossible to specifiy "
-                "'card_types' as list and 'files' as Path"
+                "Impossible to specifiy 'card_types' as list and 'files' as Path"
             )
         # Find all the json files in the given pattern
         files = [f for f in Path(files).rglob("*.json")]
     if not isinstance(card_types, list):
         card_types = [card_types for _ in files]
 
     return CardsSet.join(
-        *[
-            from_json(file, card_type)
-            for file, card_type in zip(files, card_types)
-        ]
+        *[from_json(file, card_type) for file, card_type in zip(files, card_types)]
     )
```

### Comparing `pygame_cards-0.1.2/pygame_cards/io/utils.py` & `pygame_cards-0.1.3/pygame_cards/io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 
 def key_to_json(key: Any) -> Any:
     _logger.debug(f"key_to_json: Converting {key}")
     try:
         key = str(key)
         return key
     except Exception as e:
-        raise TypeError(
-            "Could not convert {key} to a str for being a json valid key."
-        )
+        raise TypeError("Could not convert {key} to a str for being a json valid key.")
 
 
 def item_to_json(item: Any) -> Any:
     """Convert an item to a json."""
     _logger.debug(f"item_to_json: Converting type {type(item)} ")
     _logger.debug(f"item_to_json: Converting {item} ")
     if isinstance(item, (int, str, float, bool, NoneType)):
@@ -40,17 +38,15 @@
         json_item = list_to_json(item)
     elif isinstance(item, AbstractCard):
         json_item = dic_to_json(item.__dict__)
         json_item.pop("u_id")  # Remove the id as will not be used in json
     elif isinstance(item, logging.Logger):
         json_item = None
     elif hasattr(item, "__dict__"):
-        _logger.debug(
-            f"item_to_json: Found __dict__, now try converting {item} "
-        )
+        _logger.debug(f"item_to_json: Found __dict__, now try converting {item} ")
         json_item = dic_to_json(item.__dict__)
     else:
         _logger.exception(f"No conversion defined for object {item}")
         json_item = None
     _logger.debug(f"item_to_json: converted {item} to {json_item}")
 
     return json_item
```

### Comparing `pygame_cards-0.1.2/LICENSE` & `pygame_cards-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_cards-0.1.2/pyproject.toml` & `pygame_cards-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pygame_cards"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Lionel42", email="lionel@sciencegames.ch" },
 ]
 description = "Framework for simple cards games powered by Pygame"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
@@ -23,7 +23,17 @@
     "pygame_emojis",
     "numpy"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ScienceGamez/pygame_cards"
 "Bug Tracker" = "https://github.com/ScienceGamez/pygame_cards/issues"
+"Documentation" = "https://pygame-cards.readthedocs.io/en/latest/"
+
+[project.optional-dependencies]
+doc = [
+    "sphinx",
+    "furo"
+]
+
+[tool.setuptools.package-data]
+"pygame_cards.images" = ["*.png"]
```

### Comparing `pygame_cards-0.1.2/PKG-INFO` & `pygame_cards-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: pygame_cards
-Version: 0.1.2
+Version: 0.1.3
 Summary: Framework for simple cards games powered by Pygame
-Project-URL: Homepage, https://github.com/ScienceGamez/pygame_cards
-Project-URL: Bug Tracker, https://github.com/ScienceGamez/pygame_cards/issues
 Author-email: Lionel42 <lionel@sciencegames.ch>
 License: MIT License
         
         Copyright (c) 2022 ScienceGamez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,28 +20,28 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-License-File: LICENSE
+        
+Project-URL: Homepage, https://github.com/ScienceGamez/pygame_cards
+Project-URL: Bug Tracker, https://github.com/ScienceGamez/pygame_cards/issues
+Project-URL: Documentation, https://pygame-cards.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: numpy
-Requires-Dist: pygame
-Requires-Dist: pygame-emojis
 Description-Content-Type: text/markdown
+Provides-Extra: doc
+License-File: LICENSE
 
 # Pygame Cards
 
 A simple card games for pygame.
 
 Handles graphics and interaction with the mouse and pygame events.
 
-You can check our official documentation:
-
-pygame-cards.readthedocs.io
+You can check [our official documentation](https://pygame-cards.readthedocs.io)
 
 [![Documentation Status](https://readthedocs.org/projects/pygame-cards/badge/?version=latest)](https://pygame-cards.readthedocs.io/en/latest/?badge=latest)
```

