# Comparing `tmp/nsdotpy-1.2.0.tar.gz` & `tmp/nsdotpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.0.tar", max compression
+gzip compressed data, was "nsdotpy-1.2.1.tar", max compression
```

## Comparing `nsdotpy-1.2.0.tar` & `nsdotpy-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.2.0/LICENSE.md
--rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.2.0/nsdotpy/__init__.py
--rw-r--r--   0        0        0    37587 2023-05-08 19:27:31.278907 nsdotpy-1.2.0/nsdotpy/session.py
--rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.2.0/nsdotpy/valid_tags.py
--rw-r--r--   0        0        0      695 2023-05-08 19:30:24.648981 nsdotpy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2455 2023-05-08 19:30:57.675819 nsdotpy-1.2.0/README.md
--rw-r--r--   0        0        0     3282 1970-01-01 00:00:00.000000 nsdotpy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.2.1/LICENSE.md
+-rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.2.1/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    37845 2023-05-08 22:05:08.796252 nsdotpy-1.2.1/nsdotpy/session.py
+-rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.2.1/nsdotpy/valid_tags.py
+-rw-r--r--   0        0        0      695 2023-05-08 22:05:55.975348 nsdotpy-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2455 2023-05-08 22:01:45.835316 nsdotpy-1.2.1/README.md
+-rw-r--r--   0        0        0     3282 1970-01-01 00:00:00.000000 nsdotpy-1.2.1/PKG-INFO
```

### Comparing `nsdotpy-1.2.0/LICENSE.md` & `nsdotpy-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.0/nsdotpy/__init__.py` & `nsdotpy-1.2.1/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.0/nsdotpy/session.py` & `nsdotpy-1.2.1/nsdotpy/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.0"
+        self.VERSION = "1.2.1"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -843,80 +843,76 @@
         response = self.request(url, data)
         return "Region Tags updated!" in response.text
 
     # end methods for region control
 
     def junk_card(self, id: str, season: str) -> bool:
         """Junks a card from the current nation's deck.
-
         Args:
             id (str): ID of the card to junk
             season (str): Season of the card to junk
-
         Returns:
             bool: Whether the card was successfully junked or not
         """
         self.logger.info(f"Junking card {id} from season {season}")
         url = "https://www.nationstates.net/template-overall=none/page=deck"
 
         data = {"page": "ajax3", "a": "junkcard", "card": id, "season": season}
         response = self.request(url, data)
 
         return "Your Deck" in response.text
 
-    #    def open_pack(self) -> bool:
-    #        """Opens a card pack.
-    #
-    #        Returns:
-    #            bool: Whether the pack was successfully opened or not
-    #        """
-    #        cards = []
-    #        self.logger.info(f"Opening pack {each} of {count}")
-    #        url = "https://www.nationstates.net/template-overall=none/page=deck"
-    #
-    #        data = {"open_loot_box": "1"}
-    #        response = self.request(url, data)
-    #        return "Tap cards to reveal..." in response.text
-    #
-    #    def ask(self, price: str, card_id: str, season: str) -> bool:
-    #        """Asks a price on a card in a season
-    #
-    #        Args:
-    #            price (str): Price to ask
-    #            card_id (str): ID of the card
-    #            season (str): Season of the card
-    #
-    #        Returns:
-    #            bool: Whether theask was successfully lodged or not
-    #        """
-    #        self.logger.info(f"Asking for {price} on {card_id} season {season}")
-    #        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
-    #
-    #        data = {"auction_ask": price, "auction_submit": ask}
-    #        response = self.request(url, data)
-    #        return f"Your ask of {price} has been lodged." in response.text
-    #
-    #    def bid(self, price: str, card_id: str, season: str) -> bool:
-    #        """Places a bid on a card in a season
-    #
-    #        Args:
-    #            price (str): Amount of bank to bid
-    #            card_id (str): ID of the card
-    #            season (str): Season of the card
-    #
-    #        Returns:
-    #            bool: Whether the bid was successfully lodged or not
-    #        """
-    #        self.logger.info(f"Putting a bid for {price} on {card_id} season {season}")
-    #        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
-    #
-    #        data = {"auction_bid": price, "auction_submit": bid}
-    #        response = self.request(url, data)
-    #
-    #        return f"Your bid of {price} has been lodged." in response.text
+    def open_pack(self) -> bool:
+        """Opens a card pack.
+
+        Returns:
+            bool: Whether the bid was successfully removed or not
+        """
+        self.logger.info("Opening trading card pack")
+        url = "https://www.nationstates.net/template-overall=none/page=deck"
+        data = {"open_loot_box": "1"}
+        response = self.request(url, data)
+        return "Tap cards to reveal..." in response.text
+
+    def ask(self, price: str, card_id: str, season: str) -> bool:
+        """Puts an ask at price on a card in a season
+
+        Args:
+            price (str): Price to ask
+            card_id (str): ID of the card
+            season (str): Season of the card
+
+        Returns:
+            bool: Whether the ask was successfully lodged or not
+        """
+        self.logger.info(f"Asking for {price} on {card_id} season {season}")
+        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+
+        data = {"auction_ask": price, "auction_submit": "ask"}
+        response = self.request(url, data)
+        return f"Your ask of {price} has been lodged." in response.text
+
+    def bid(self, price: str, card_id: str, season: str) -> bool:
+        """Places a bid on a card in a season
+
+        Args:
+            price (str): Amount of bank to bid
+            card_id (str): ID of the card
+            season (str): Season of the card
+
+        Returns:
+            bool: Whether the bid was successfully lodged or not
+        """
+        self.logger.info(f"Putting a bid for {price} on {card_id} season {season}")
+        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+
+        data = {"auction_bid": price, "auction_submit": "bid"}
+        response = self.request(url, data)
+
+        return f"Your bid of {price} has been lodged." in response.text
 
     def remove_ask(self, price: str, card_id: str, season: str) -> bool:
         """Removes an ask on card_id in season at price
 
         Args:
             price (str): Price of the ask to remove
             card_id (str): ID of the card
@@ -931,28 +927,42 @@
 
         data = {"new_price": price, "remove_ask_price": price}
         response = self.request(url, data)
         return f"Removed your ask for {price}" in response.text
 
     def remove_bid(self, price: str, card_id: str, season: str) -> bool:
         """Removes a big on a card
-
         Args:
             price (str): Price of the bid to remove
             card_id (str): ID of the card
             season (str): Season of the card
-
         Returns:
             bool: Whether the bid was successfully removed or not
         """
 
         self.logger.info(f"Removing a bid for {price} on {card_id} season {season}")
         url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
 
         data = {"new_price": price, "remove_bid_price": price}
         response = self.request(url, data)
 
         return f"Removed your bid for {price}" in response.text
 
+    def expand_deck(self, price: str) -> bool:
+        """Upgrades deck capcity
+        Args:
+            price (str): Price of the Upgrade
+        Returns:
+            bool: Whether the upgrade was successfully removed or not
+        """
+
+        self.logger.info(f"Upgrading your deck at a cost of {price}")
+        url = "https://www.nationstates.net/page=deck"
+
+        data = {"embiggen_deck": price}
+        response = self.request(url, data)
+
+        return f"Increased deck capacity from" in response.text
+
 
 if __name__ == "__main__":
     print("this is a module/library, not a script")
```

### Comparing `nsdotpy-1.2.0/nsdotpy/valid_tags.py` & `nsdotpy-1.2.1/nsdotpy/valid_tags.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.0/pyproject.toml` & `nsdotpy-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.0"
+version = "1.2.1"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.2.0/README.md` & `nsdotpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.0/PKG-INFO` & `nsdotpy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

