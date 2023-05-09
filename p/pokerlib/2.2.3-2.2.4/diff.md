# Comparing `tmp/pokerlib-2.2.3.tar.gz` & `tmp/pokerlib-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.2.3.tar", max compression
+gzip compressed data, was "pokerlib-2.2.4.tar", max compression
```

## Comparing `pokerlib-2.2.3.tar` & `pokerlib-2.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.3/LICENSE
--rw-r--r--   0        0        0     5980 2023-05-05 21:16:26.697525 pokerlib-2.2.3/README.md
--rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.3/pokerlib/__init__.py
--rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/_handparser.py
--rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/_player.py
--rw-r--r--   0        0        0    17750 2023-05-06 18:50:56.359624 pokerlib-2.2.3/pokerlib/_round.py
--rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.3/pokerlib/_table.py
--rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/enums.py
--rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/implementations/_no_muck_showdown_table.py
--rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/implementations/_no_muck_table.py
--rw-r--r--   0        0        0      663 2023-05-06 18:52:00.259619 pokerlib-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 pokerlib-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.4/LICENSE
+-rw-r--r--   0        0        0     5980 2023-05-05 21:16:26.697525 pokerlib-2.2.4/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.4/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/_player.py
+-rw-r--r--   0        0        0    17944 2023-05-08 12:46:59.828312 pokerlib-2.2.4/pokerlib/_round.py
+-rw-r--r--   0        0        0     6937 2023-05-08 12:36:12.798296 pokerlib-2.2.4/pokerlib/_table.py
+-rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/enums.py
+-rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-05-09 16:39:25.052221 pokerlib-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 pokerlib-2.2.4/PKG-INFO
```

### Comparing `pokerlib-2.2.3/LICENSE` & `pokerlib-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.3/README.md` & `pokerlib-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.3/pokerlib/_handparser.py` & `pokerlib-2.2.4/pokerlib/_handparser.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.3/pokerlib/_player.py` & `pokerlib-2.2.4/pokerlib/_player.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.3/pokerlib/_round.py` & `pokerlib-2.2.4/pokerlib/_round.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self.closed = False
 
         self.small_blind = small_blind
         self.big_blind = big_blind
 
         self.players = players
         self.button = button
-        self.current_index = button # it will move
+        self.current_index = self.starting_player_index
 
         self.board = list()
         self.turn = None
 
         self._deck = self._deckIterator()
         self._turn_generator = self._turnGenerator()
         self._muck_optioned_player_ids = []
@@ -182,15 +182,16 @@
                 player.id,
                 self.PrivateOutId.DEALTCARDS
             )
 
         next(self._turn_generator)
         self._dealSmallBlind()
         self._dealBigBlind()
-        self._postActionStateUpdate()
+        self._postActionStateUpdate(False)
+        self._requireAction()
 
     def _dealSmallBlind(self):
         small_blind_player = self.players[self.small_blind_player_index]
         paid_amount = self._addToPot(small_blind_player, self.small_blind)
         self.publicOut(
             self.PublicOutId.SMALLBLIND,
             player_id = small_blind_player.id,
@@ -288,28 +289,27 @@
             else:
                 self._muck_optioned_player_ids.append(player.id)
                 self.publicOut(
                     self.PublicOutId.PLAYERCHOICEREQUIRED,
                     player_id = player.id,
                 )
 
-    def _shiftCurrentPlayer(self):
-        self.current_index = self.players.nextActiveIndex(
-            self.current_index)
-
-    def _moveToNextPlayer(self):
-        self._shiftCurrentPlayer()
+    def _requireAction(self):
         called = self.current_player.turn_stake[self.turn]
         self.publicOut(
             self.PublicOutId.PLAYERACTIONREQUIRED,
             player_id = self.current_player.id,
             to_call = self.turn_stake - called
         )
 
-    def _postActionStateUpdate(self, is_update_after_forcefold=False):
+    def _shiftCurrentPlayer(self):
+        self.current_index = self.players.nextActiveIndex(
+            self.current_index)
+
+    def _postActionStateUpdate(self, move_to_new_player=True):
         active = self.players.countActivePlayers()
         not_folded = self.players.countUnfoldedPlayers()
         pots_balanced = self._potsBalanced()
 
         if not_folded == 0:
             return self._close()
 
@@ -324,22 +324,25 @@
 
         elif self.players.allPlayedTurn() and pots_balanced:
             if self.turn == Turn.RIVER:
                 self._dealWinnings()
                 return self._finish()
             else:
                 next(self._turn_generator)
-                self.current_index = self.button
-                return self._moveToNextPlayer()
+                self.current_index = self.starting_player_index
+                return self._requireAction()
 
-        # this function can be called after a non-current-player's
-        # hand is force-folded, in which case we don't want to move
-        # onto the next player
-        elif not is_update_after_forcefold:
-            self._moveToNextPlayer()
+        # this function is usually called after a player's action,
+        # in which case it should move on to next active player,
+        # but if called before flop, it should not move from the
+        # starting player index. Also, if a hand is force-folded
+        # from non-current player we don't want to move the player
+        elif move_to_new_player:
+            self._shiftCurrentPlayer()
+            self._requireAction()
 
     def _fold(self):
         self.current_player.is_folded = True
         self.publicOut(
             self.PublicOutId.PLAYERFOLD,
             player_id = self.current_player.id
         )
```

### Comparing `pokerlib-2.2.3/pokerlib/_table.py` & `pokerlib-2.2.4/pokerlib/_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         if self.round and player in self.round:
             if player.id == self.round.current_player.id:
                 self.round.publicIn(
                     player.id, self.RoundClass.PublicInId.FOLD
                 )
             else:
                 player.is_folded = True
-                self.round._postActionStateUpdate(True)
+                self.round._postActionStateUpdate(False)
         # notify that player was removed from table
         self.publicOut(
             self.PublicOutId.PLAYERREMOVED,
             player_id = player.id,
         )
 
     def _newRound(self, round_id):
```

### Comparing `pokerlib-2.2.3/pokerlib/enums.py` & `pokerlib-2.2.4/pokerlib/enums.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.3/pyproject.toml` & `pokerlib-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.2.3"
+version = "2.2.4"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.2.3/PKG-INFO` & `pokerlib-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerlib
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python poker library
 Home-page: https://github.com/kuco23/pokerlib/
 Keywords: python,poker,library
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

