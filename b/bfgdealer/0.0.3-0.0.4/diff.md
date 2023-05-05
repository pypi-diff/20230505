# Comparing `tmp/bfgdealer-0.0.3.tar.gz` & `tmp/bfgdealer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgdealer-0.0.3.tar", last modified: Tue Mar 14 09:16:40 2023, max compression
+gzip compressed data, was "bfgdealer-0.0.4.tar", last modified: Fri May  5 16:15:21 2023, max compression
```

## Comparing `bfgdealer-0.0.3.tar` & `bfgdealer-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-14 09:16:40.540764 bfgdealer-0.0.3/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.3/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      837 2023-03-14 09:16:40.540764 bfgdealer-0.0.3/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.3/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-14 09:16:40.537431 bfgdealer-0.0.3/bfgdealer/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-02-01 12:53:06.000000 bfgdealer-0.0.3/bfgdealer/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       31 2023-03-14 09:13:10.000000 bfgdealer-0.0.3/bfgdealer/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-14 09:16:40.540764 bfgdealer-0.0.3/bfgdealer/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.3/bfgdealer/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    19984 2023-03-08 17:58:50.000000 bfgdealer-0.0.3/bfgdealer/source/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10494 2023-02-01 13:00:46.000000 bfgdealer-0.0.3/bfgdealer/source/dealer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    28311 2023-03-14 09:13:10.000000 bfgdealer-0.0.3/bfgdealer/source/dealer_duo.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.3/bfgdealer/source/dealer_engine.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    15690 2023-03-05 10:44:23.000000 bfgdealer-0.0.3/bfgdealer/source/dealer_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-14 09:16:40.537431 bfgdealer-0.0.3/bfgdealer.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      837 2023-03-14 09:16:40.000000 bfgdealer-0.0.3/bfgdealer.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-03-14 09:16:40.000000 bfgdealer-0.0.3/bfgdealer.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-03-14 09:16:40.000000 bfgdealer-0.0.3/bfgdealer.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-03-14 09:16:40.000000 bfgdealer-0.0.3/bfgdealer.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-03-14 09:16:40.540764 bfgdealer-0.0.3/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.3/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.4/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.4/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.918158 bfgdealer-0.0.4/bfgdealer/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-02-01 12:53:06.000000 bfgdealer-0.0.4/bfgdealer/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       31 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/bfgdealer/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.4/bfgdealer/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    20266 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    10586 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/dealer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    27456 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/dealer_duo.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.4/bfgdealer/source/dealer_engine.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14324 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/dealer_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.918158 bfgdealer-0.0.4/bfgdealer.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.4/setup.py
```

### Comparing `bfgdealer-0.0.3/LICENSE.txt` & `bfgdealer-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.3/PKG-INFO` & `bfgdealer-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.3
+Version: 0.0.4
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.4 05 May 2023
+
+1. Change set hands defn
+
+------
+
 Version 0.0.3 14 Mar 2023
 
 1. Improve condition checking on negative doubles
 
 ------
 
 Version 0.0.2 08 Mar 2023
```

### Comparing `bfgdealer-0.0.3/bfgdealer/source/board.py` & `bfgdealer-0.0.4/bfgdealer/source/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
+"""Auction
     Board class extends bridgeobjects Board
 """
 
 from datetime import datetime
 import json
 from termcolor import cprint
 
 from bfgbidding import Player, Hand
 from bridgeobjects import (Board as bfg_Board, RANKS, SEATS, SUITS,
                             parse_pbn, Contract,
                             Auction, Trick)
 
 
-MODULE_COLOUR = 'blue'
+MODULE_COLOUR = 'green'
 
 DEFAULT_SUIT_ORDER = ['S', 'H', 'C', 'D']
 
 
 class Board(bfg_Board):
     """Define BfG Board class."""
     def __init__(self, *args, **kwargs):
@@ -343,36 +343,46 @@
         if not self._auction:
             return contract
 
         if not (self._three_final_passes(self._auction.calls) and
                 not self._passed_out(self._auction.calls)):
             return contract
 
-        dealer_index = SEATS.index(self.dealer)
+        (call, modifier, declarer_partition) = self._analyse_auction()
+
+        declarer_index = self._get_declarer_index(call, declarer_partition)
+        declarer = SEATS[declarer_index]
+        contract = Contract(f'{call.name}{modifier}', declarer)
+        return contract
+
+    def _analyse_auction(self):
         auction_calls = [call for call in self._auction.calls]
         auction_calls.reverse()
         modifier = ''
         for call in auction_calls:
             if call.name == 'R':
                 modifier = 'R'
-            if not modifier and call.name == 'D':
+            if call.name == 'D':
                 modifier = 'D'
             if call.is_value_call:
                 break
-        denomination = call.denomination
         declarer_partition = self._auction.calls.index(call)
 
+        return (call, modifier, declarer_partition)
+
+    def _get_declarer_index(self, call, declarer_partition):
         for index, check_call in enumerate(self._auction.calls):
-            if (check_call.denomination == denomination and
+            if (check_call.denomination == call.denomination and
                     (declarer_partition - index) % 2 == 0):
                 break
+        dealer_index = SEATS.index(self.dealer)
         declarer_index = (dealer_index + index) % 4
-        declarer = SEATS[declarer_index]
-        contract = Contract(f'{call.name}{modifier}', declarer)
-        return contract
+        return declarer_index
+
+
 
     @staticmethod
     def _passed_out(calls):
         """Return True if the board has been passed out."""
         if len(calls) != 4:
             return False
         for call in calls:
```

### Comparing `bfgdealer-0.0.3/bfgdealer/source/dealer.py` & `bfgdealer-0.0.4/bfgdealer/source/dealer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """The dealer object for the bridgeobjects module."""
 
 import random
+from termcolor import cprint
 
 from bridgeobjects import (SEATS, SHAPES, BALANCED_SHAPES, Call)
+from bfgbidding import Bid
 
 from .dealer_engine import DealerEngine
 from .board import Board, Auction
 
 
+MODULE_COLOUR = 'cyan'
+
 class Dealer(object):
     """The dealer object for the bridgeobjects module."""
     DEFAULT_POINTS_RANGE = [12, 14]
     #: the maximum number of points allowed in a hand
     MAX_POINTS = 26
 
     #: shapes suitable for single suited rebids
@@ -210,19 +214,20 @@
                 result = False
         return result
 
     def _generate_auction_calls(self, board):
         """Return the auction calls as a list."""
         board.auction = Auction()
         player_index = SEATS.index(board.dealer)
+        board.auction.calls = []
         while not self._three_passes(board.bid_history):
             player = board.players[player_index]
-            player.make_bid(board)
+            bid = player.make_bid(board)
+            board.auction.calls.append(bid)
             player_index = (player_index + 1) % 4
-        board.auction.calls = [Call(bid) for bid in board.bid_history]
         return board.auction.calls
 
     @staticmethod
     def _three_passes(calls):
         """Return True if there have been three consecutive passes."""
         three_passes = False
         if len(calls) >= 4:
```

### Comparing `bfgdealer-0.0.3/bfgdealer/source/dealer_duo.py` & `bfgdealer-0.0.4/bfgdealer/source/dealer_duo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,197 +1,174 @@
 import random
 from termcolor import cprint
 
 from .dealer import Dealer as DealerBase
 from bridgeobjects import SEATS, BALANCED_SHAPES, SUITS, SHAPES
 
-SET_HANDS = {
-    0: 'Weak NT',
-    1: 'Strong NT',
-    2: '5 card majors',
-    3: '20+ points hand',
-    4: '23+ points hand',
-    5: 'Benji 2C opening hand',
-    6: 'Slam potential',
-    7: 'Jacoby 2NT',
-    8: 'Negative doubles',
-    9: 'Splinters',
-    10: 'Unassuming Cue bids',
-    11: 'Take-out doubles',
-    12: 'Defending against weak 1NT',
-    13: 'Fourth suit forcing',
-    14: 'Response to preemptive opening',
-    15: 'Defending preemptive opening',
-    16: 'Support for a minor',
-    17: 'Multi-2D',
-}
-
 MODULE_COLOUR = 'red'
 
-
 class Dealer(DealerBase):
     """Generate deals for Duo stages."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+
+        self.set_hands = [
+            ('Weak NT', self.weak_nt_hand),
+            ('Strong NT', self.strong_nt_hand),
+            # ('5 card majors', self.five_card_major_opening),
+            ('20+ points hand', self.twenty_plus_hand),
+            ('23+ points hand', self.twenty_three_plus_hand),
+            ('Benji 2C opening hand', self.benji_two_club_hand),
+            ('Slam potential', self.slam_potential_hand),
+            ('Jacoby 2NT', self.jacoby_2nt_board),
+            ('Negative doubles', self.negative_double_hand),
+            ('Splinters', self.splinter_board),
+            ('Unassuming cue bids', self.unassuming_cue_bid_board),
+            ('Take-out doubles', self.take_out_double_board),
+            ('Defending against weak 1NT', self.defend_weak_nt_board),
+            ('Fourth suit forcing', self.fourth_suit_forcing_board),
+            ('Response to preemptive opening', self.respond_to_preempt_board),
+            ('Defending preemptive opening', self.defend_preempt_board),
+            ('Support for a minor', self.minor_support_board),
+            ('Multi-2D', self.multi_two_diamond),
+        ]
         self.generate_hand = self.engine.get_hand_from_points_and_shape
+        self.create_board = self.engine.create_board_from_hands
+        self.random_shape = self.engine.select_random_shape_from_list
         self._dealer = ''
 
     def get_set_hand(self, stages, dealer):
         """Return a board relevant to set stages."""
         self._dealer = dealer
-
         stage = int(random.choice(stages))
-        # Duo hands
-        if stage == 0:  # Weak NT
-            board = self.weak_nt_hand()
-        elif stage == 1:  # Strong NT:
-            board = self.strong_nt_hand()
-        elif stage == 2:  # 5 card majors
-            board = self.five_card_major_opening()
-        elif stage == 3:  # 20+ points hand
-            board = self.twenty_plus_hand()
-        elif stage == 4:  # 23+ points hand
-            board = self.twenty_three_plus_hand()
-        elif stage == 5:  # Benji 2C opening hand
-            board = self.benji_two_club_hand()
-        elif stage == 6:  # Slam potential
-            board = self.slam_potential_hand()
-        elif stage == 7:  # Jacoby 2NT
-            board = self.jacoby_2nt_board()
-        elif stage == 8:  # Negative doubles
-            board = self.negative_double_hand()
-        elif stage == 9:  # Splinters
-            board = self.splinter_board()
-        elif stage == 10:  # Unassuming Cue bids
-            board = self.unassuming_cue_bid_board()
-        elif stage == 11:  # Take-out doubles
-            board = self.take_out_double_board()
-        elif stage == 12:  # Defending weak 1N
-            board = self.defend_weak_nt_board()
-        elif stage == 13:  # Fourth suit forcing
-            board = self.fourth_suit_forcing_board()
-        elif stage == 14:  # Response to preemptive opening
-            board = self.respond_to_preempt_board()
-        elif stage == 15:  # Defending preemptive opening
-            board = self.defend_preempt_board()
-        elif stage == 16:  # Support for a minor
-            board = self.minor_support_board()
-        elif stage == 17:  # Multi-2D
-            board = self.multi_two_diamond()
-        elif stage == 99:  # xxx
-            board = self.deal_random_board()
-        else:
-            board = self.deal_random_board()
+        board = self.set_hands[stage][1]()
         board.dealer = self._dealer
         board.stage = stage
         return board
 
     def _first_seat(self):
         if self._dealer in 'EW':
             return (SEATS.index(self._dealer) + 1) % 4
         return SEATS.index(self._dealer)
 
     def twenty_plus_hand(self):
         """Return a board with 20+ points."""
         hand = self.generate_hand([20, 35])
         hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         return board
 
     def twenty_three_plus_hand(self):
         """Return a board with 20+ points."""
         hand = self.generate_hand([23, 35])
         hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         return board
 
     def weak_nt_hand(self):
         """Deal a balanced hand with 12-14 points."""
         hand = self.generate_hand([12, 14], BALANCED_SHAPES)
         hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         return board
 
     def strong_nt_hand(self):
         """Deal a balanced hand with 15-17 points."""
         hand = self.generate_hand([15, 17], BALANCED_SHAPES)
         hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         return board
 
     def five_card_major_opening(self):
         """Deal a hand with 5 card major 12 + points."""
         found = False
         hand = None
         while not found:
             hand = self.generate_hand([12, 35])
             if hand.spades >= 5 or hand.hearts >= 5:
                 found = True
         hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         return board
 
     def benji_two_club_hand(self):
-        """Deal a hand with Benji 2C opener."""
+        """
+            Deal a hand with Benji 2C opener.
+
+            Either balanced 19-20 or
+            long suit 16-22.
+        """
+        hand = self._get_benji_hand()
+        hands = {self._first_seat(): hand}
+        board = self.create_board(hands)
+        return board
+
+    def _get_benji_hand(self):
         selection = random.randint(0, 2)
         hand = None
         if selection == 2:
-            hand = self.generate_hand([19, 20], BALANCED_SHAPES)
-        else:
-            found = False
-            while not found:
-                hand = self.generate_hand([16,22], self.WEAK_TWO_SHAPES)
-                if hand.suit_points(hand.longest_suit) >= 8:
-                    if not (hand.shape[0] == 6 and hand.aces < 2):
-                        found = True
-        hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
-        return board
+            return self.generate_hand([19, 20], BALANCED_SHAPES)
+
+        while True:
+            hand = self.generate_hand([16,22], self.WEAK_TWO_SHAPES)
+            if hand.suit_points(hand.longest_suit) >= 9:
+                if (hand.shape[0] != 6 and hand.aces < 2):
+                    return hand
 
     def slam_potential_hand(self):
         """Deal a hand with slam potential."""
         found = False
         board = None
         while not found:
             hand = self.generate_hand([16, 35])
             hands = {self._first_seat(): hand}
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             auction = self._generate_auction_calls(board)
             if auction[-4].level >= 6:
                 found = True
         return board
 
     def jacoby_2nt_board(self):
         """
             Deal a hand with jacoby 2NT response.
 
             The Jacoby 2NT convention is an artificial, game-forcing response to
             a 1H or 1S opening bid. The 2NT response shows 4+ trump support with
-            13+ points. The bid asks partner to describe her hand further so
+            13+ (or a good 12) points. The bid asks partner to describe her hand further so
             that slam prospects can be judged accordingly.
         """
         found = False
         board = None
         while not found:
             openers_hand = self.generate_hand([12, 19])
             opener = self._first_seat()
             responder = (opener + 2) % 4
             hands = {opener: openers_hand}
             if openers_hand.spades < 4 and openers_hand.hearts < 4:
                 continue
             if openers_hand.shape[0] == 4 and openers_hand.hcp <= 14:
                 continue
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
+
+            # board.dealer = self._dealer
+            # cprint(f"{board.dealer}", MODULE_COLOUR)
+            auction = self._generate_auction_calls(board)
+            if self._dealer in 'EW': # and auction.calls[0].name != 'P':
+                auction_2 = self._generate_auction_calls(board)
+                # cprint(f"{board.dealer=}", MODULE_COLOUR)
+                # cprint(f"{auction}", MODULE_COLOUR)
+                # cprint(f"{auction_2}", 'green')
+                # continue
+
             partners_hand = board.hands[responder]
             if partners_hand.spades < 4 and partners_hand.hearts < 4:
                 continue
             if not (partners_hand.hcp >= 12 and partners_hand.shape[3] >= 2):
                 continue
-            auction = self._generate_auction_calls(board)
             if self._four_of_openers_major(partners_hand, auction):
                 found = True
         return board
 
     @staticmethod
     def _four_of_openers_major(partner, auction):
         """Return True if hand has 4 of partner's major."""
@@ -390,15 +367,15 @@
         # The first hand to bid on NS gets the opening hand.
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=True)
         del check_bid
         hands = {
             opener: openers_hand,
             responder: responders_hand,
         }
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         board.dealer = self._dealer
         return (board, opener)
 
     @staticmethod
     def _get_distribution_points(hand):
         """Return the distribution points for a hand."""
         distribution_points = 0
@@ -467,15 +444,15 @@
         dealer_index = SEATS.index(self._dealer)
         while not found:
             (board, opener) = self._get_opener_overcaller_board(ns_opener=False)
             hands = {
                 opener: board.hands[opener],
             }
             # generate a new board where either N or S might be overcaller.
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = self._dealer
 
             # These checks seem to slow it down!
             # Responders hand
             responder = (opener + 2) % 4
             # responders_hand = board.hands[responder]
             # if responders_hand.hcp < 11:
@@ -535,15 +512,15 @@
         del responder
         overcaller = (opener + 1) % 4
 
         while not found:
             hand = self.generate_hand([12, 14], BALANCED_SHAPES)
             hands = {opener: hand,}
             # generate a new board where E or W open 1NT.
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = self._dealer
 
             auction = self._generate_auction_calls(board)
             if auction[check_bid].name != '1NT':
                 found = False
             elif board.hands[overcaller].hcp < 9 or board.hands[overcaller].shape[0] < 5:
                 found = False
@@ -558,15 +535,15 @@
 
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=True)
         del responder
 
         while not found:
             hand = self.generate_hand([12, 19])
             hands = {opener: hand,}
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = self._dealer
             auction = self._generate_auction_calls(board)
 
             denominations = []
             nt_bid = False
             for index, call in enumerate(auction):
                 # Get a list of suits called in the auction by N/S
@@ -591,15 +568,15 @@
     def respond_to_preempt_board(self):
         """Generate a board to test response to a preemptive opening."""
         found = False
         board = None
 
         # Get shape and points range
         shapes = [shape for shape in SHAPES if shape[0] >= 6]
-        shape = self.engine.select_random_shape_from_list(shapes)
+        shape = self.random_shape(shapes)
         if shape[0] == 6:
             points = [6, 9]
         else:
             points = [0, 9]
 
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=True)
 
@@ -608,15 +585,15 @@
             if openers_hand.suit_length(SUITS['C']) >=6:
                 continue
             responders_hand = self.generate_hand([14, 25], partners_hand=openers_hand)
             hands = {
                 opener: openers_hand,
                 responder: responders_hand,
                 }
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = self._dealer
             auction = self._generate_auction_calls(board)
 
             # Check first bid is valid
             call = auction[check_bid]
             if call.level in (2, 3, 4):
                 found = True
@@ -625,15 +602,15 @@
     def defend_preempt_board(self):
         """Generate a board to test response to a preemptive opening."""
         found = False
         board = None
 
         # Get shape and points range
         shapes = [shape for shape in SHAPES if shape[0] >= 6]
-        shape = self.engine.select_random_shape_from_list(shapes)
+        shape = self.random_shape(shapes)
         if shape[0] == 6:
             points = [6, 9]
         else:
             points = [0, 9]
 
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=False)
 
@@ -642,15 +619,15 @@
             if openers_hand.suit_length(SUITS['C']) == 6:
                 continue
             responders_hand = self.generate_hand([0, 8], partners_hand=openers_hand)
             hands = {
                 opener: openers_hand,
                 responder: responders_hand,
                 }
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = self._dealer
             auction = self._generate_auction_calls(board)
 
             # Check first bid is valid
             if check_bid:
                 if auction[0].name  != 'P':
                     continue
@@ -668,15 +645,15 @@
             responders_min_points = 25 - openers_hand.hcp
             responders_points = [responders_min_points, 19]
             responders_hand = self.generate_hand(responders_points, partners_hand=openers_hand)
             hands = {
                 opener: openers_hand,
                 responder: responders_hand,
                 }
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = self._dealer
             auction = self._generate_auction_calls(board)
 
             # Check first bid is valid
             if check_bid:
                 if auction[0].name  != 'P':
                     continue
@@ -686,15 +663,15 @@
                     found = True
         return board
 
     def multi_two_diamond(self):
         # TODO ...
         hand = self.generate_hand([20, 35])
         hands = {self._first_seat(): hand}
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         return board
 
 
     def _opener_given_dealer(self, ns_opener):
         """Return the seat indices given dealer and opener orientation."""
         # E.g if we want N or S to bid and E is dealer then the opener will be S.
         # If on the other hand W is dealer, the opener will be N.
@@ -721,15 +698,15 @@
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener)
         del check_bid, responder
         overcaller = (opener + 1) % 4
         hands = {
             opener: openers_hand,
             overcaller: overcallers_hand,
         }
-        board = self.engine.create_board_from_hands(hands)
+        board = self.create_board(hands)
         board.dealer = self._dealer
         return (board, opener)
 
     @staticmethod
     def _opener_is_ns(auction, openers_call):
         """Return True if N or S make the first bid."""
         for index in range(openers_call):
```

### Comparing `bfgdealer-0.0.3/bfgdealer/source/dealer_engine.py` & `bfgdealer-0.0.4/bfgdealer/source/dealer_engine.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.3/bfgdealer/source/dealer_solo.py` & `bfgdealer-0.0.4/bfgdealer/source/dealer_solo.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,198 +3,172 @@
 
 from bridgeobjects import SEATS, BALANCED_SHAPES, SEMI_BALANCED_SHAPES, Call
 
 from .dealer import Dealer as DealerBase, Board
 
 MODULE_COLOUR = 'green'
 
-
-SET_HANDS = {
-    0: 'Opening ones',
-    1: 'Limit bids',
-    2: 'Response in new suit',
-    3: 'Balanced rebids',
-    4: 'Single suited rebids',
-    5: 'Two suited rebids',
-    6: 'Support for responder',
-    # 'Raise responders NT',
-    8: 'Response to weak two',
-    9: 'Response to 2NT',
-    10: 'Response to 2C',
-}
-
 class Dealer(DealerBase):
     """Generate deals for Solo stages."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        self.set_hands = [
+            ('Opening ones', self.opening_one_board),
+            ('Limit bids', self.limit_bids_responder_board),
+            ('Response in new suit', self.respond_in_new_suit_board),
+            ('Balanced rebids', self.balanced_rebid_board),
+            ('Single suited rebids', self.single_suited_rebid_board),
+            ('Two suited rebids', self.two_suited_rebid_board),
+            ('Support for responder', self.support_for_responder_board),
+            ('Response to weak two', self.response_to_weak_two_board),
+            ('Response to 2NT', self.response_to_two_nt_board),
+            ('Response to 2C', self.response_to_two_clubs_board),
+        ]
+        self.generate_hand = self.engine.get_hand_from_points_and_shape
+        self.create_board = self.engine.create_board_from_hands
+
     def get_set_hand(self, stages, seat):
         """Return a board relevant to set stages."""
-
         seat_index = SEATS.index(seat)
         stage = int(random.choice(stages))
-
-        # Solo hands
-        if stage == 0:  #  Opening ones
-            board = self.deal_opening_one_board(seat_index)
-        elif stage == 1:  #  Limit bids
-            board = self.deal_limit_bids_responder_board(seat_index)
-        elif stage == 2:  #  Response in new suit
-            board = self.deal_respond_in_new_suit_board(seat_index)
-        elif stage == 3:  #  Balanced rebids
-            board = self.deal_balanced_rebid_board(seat_index)
-        elif stage == 4:  #  Single suited rebids
-            board = self.deal_single_suited_rebid_board(seat_index)
-        elif stage == 5:  #  Two suited rebids
-            board = self.deal_two_suited_rebid_board(seat_index)
-        elif stage == 6:  #  Support for responder
-            board = self.deal_support_for_responder_board(seat_index)
-        elif stage == 7:  #  Raise responders NT
-            board = self.deal_raise_responder_nt_board(seat_index)
-        elif stage == 8:  #  Response to weak two
-            board = self.deal_response_to_weak_two_board(seat_index)
-        elif stage == 9:  #  Response to 2NT
-            board = self.deal_response_to_two_nt_board(seat_index)
-        elif stage == 10:  #  Response to 2C
-            board = self.deal_response_to_two_clubs_board(seat_index)
-        else:
-            board = self.deal_random_board()
+        board = self.set_hands[stage][1](seat_index)
         board.stage = stage
         return board
 
-    def deal_opening_one_board(self, seat_index):
+    def opening_one_board(self, seat_index):
         """Return a board suitable for an opening one."""
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
-            openers_hand = self.engine.get_hand_from_points_and_shape([12, 22])
+            openers_hand = self.generate_hand([12, 22])
             hands = {seat_index: openers_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[seat_index])
+            board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
             auction = self._generate_auction_calls(board)
             if auction[0].level == 1 and self._valid_overcalls(auction):
                 found = True
         return board
 
-    def deal_limit_bids_responder_board(self, seat_index):
+    def limit_bids_responder_board(self, seat_index):
         """Return a board suitable for limited responses to opener."""
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
-            openers_hand = self.deal_opening_one_hand()
+            openers_hand = self.opening_one_hand()
             if (openers_hand.shape in BALANCED_SHAPES and
                     openers_hand.high_card_points <= 14):
                 responders_hand = self._deal_limit_bids_responder_nt(openers_hand)
             else:
                 responders_hand = self._deal_limit_bids_responder_support(openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[partners_index])
+            board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
             auction = self._generate_auction_calls(board)
             if self._valid_overcalls(auction):
                 found = True
         return board
 
     def _deal_limit_bids_responder_nt(self, openers_hand):
         """Return a hand suitable for an NT response after opening one."""
         shapes = BALANCED_SHAPES.extend(SEMI_BALANCED_SHAPES)
-        responders_hand = self.engine.get_hand_from_points_and_shape([0, 17], shapes, openers_hand)
+        responders_hand = self.generate_hand([0, 17], shapes, openers_hand)
         return responders_hand
 
     def _deal_limit_bids_responder_support(self, openers_hand):
         """Return a hand suitable for an NT response after opening one."""
         board = Board()
         board.hands[0] = openers_hand
         board.players[0].hand = openers_hand
         openers_bid = board.players[0].make_bid(board)
         loop = 1
         found = False
         responders_hand = None
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         while not found:
             loop += 1
             responders_hand = get_hand([3, 16], None, openers_hand)
             if (openers_bid.is_minor and
                     responders_hand.four_card_major_or_better and
                     responders_hand.hcp >= 6):
                 found = False
             elif (openers_bid.is_suit_call and
                     responders_hand.suit_holding[openers_bid.denomination] < 4):
                 found = False
             else:
                 found = True
         return responders_hand
 
-    def deal_balanced_rebid_board(self, seat_index):
+    def balanced_rebid_board(self, seat_index):
         """Return a board suitable for balanced response."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
             openers_hand = get_hand([15, 19], BALANCED_SHAPES)
             responders_hand = get_hand([3, 20], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[seat_index])
+            board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
             auction = self._generate_auction_calls(board)
             if len(auction) >= 5:
                 openers_bid = auction[0]
                 responders_bid = auction[2]
                 if (openers_bid.denomination != responders_bid.denomination and
                         not responders_bid.is_no_trumps):
                     if self._valid_overcalls(auction):
                         found = True
         return board
 
-    def deal_single_suited_rebid_board(self, seat_index):
+    def single_suited_rebid_board(self, seat_index):
         """Return a board suitable for single suit response."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
             openers_hand = get_hand([12, 19], self.SINGLE_SUITED_SHAPES)
             responders_hand = get_hand([6, 15], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[seat_index])
+            board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
             auction = self._generate_auction_calls(board)
             if len(auction) >= 5:
                 openers_bid_one = auction[0]
                 responders_bid = auction[2]
                 openers_bid_two = auction[4]
                 if (openers_bid_one.denomination == openers_bid_two.denomination and
                         responders_bid.denomination != openers_bid_one.denomination and
                         responders_bid.denomination != openers_bid_two.denomination):
                     if self._valid_overcalls(auction):
                         found = True
         return board
 
-    def deal_two_suited_rebid_board(self, seat_index):
+    def two_suited_rebid_board(self, seat_index):
         """Return a board suitable for two suit response."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         found = False
         board = None
         while not found:
             openers_hand = get_hand([12, 19], self.TWO_SUITED_SHAPES)
             responders_hand = get_hand([6, 15], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[seat_index])
+            board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
             auction = self._generate_auction_calls(board)
             openers_bid_one = auction[0]
             if len(auction) >= 5:
                 openers_bid_two = auction[4]
             else:
                 # dummy inserted to ensure a 2 level bid
@@ -221,142 +195,142 @@
                     found = True
                 else:
                     found = False
             else:
                 found = True
         return board
 
-    def deal_support_for_responder_board(self, seat_index):
+    def support_for_responder_board(self, seat_index):
         """Return a board suitable for supporting responder's suit."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         openers_hand = get_hand([12, 19], self.TWO_SUITED_SHAPES)
         loop = 1
         found = False
         board = None
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         while not found:
             loop += 1
             responders_hand = get_hand([6, 16], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[seat_index])
+            board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
             auction = self._generate_auction_calls(board)
             openers_bid = auction[0]
             responders_bid = auction[2]
             if responders_bid.is_suit_call:
                 if self._valid_overcalls(auction):
                     responders_suit = responders_bid.denomination
                     if (openers_bid.denomination != responders_suit and
                             openers_hand.suit_holding[responders_suit] >= 4):
                         found = True
         return board
 
-    def deal_respond_in_new_suit_board(self, seat_index):
+    def respond_in_new_suit_board(self, seat_index):
         """Return a board where responder bids new suit."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         openers_hand = get_hand([12, 19], self.TWO_SUITED_SHAPES)
         loop = 1
         found = False
         board = None
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         while not found:
             loop += 1
             responders_hand = get_hand([6, 16], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[partners_index])
+            board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
             auction = self._generate_auction_calls(board)
             openers_bid = auction[0]
             responders_bid = auction[2]
             if responders_bid.is_suit_call:
                 if self._valid_overcalls(auction):
                     responders_suit = responders_bid.denomination
                     if openers_bid.denomination != responders_suit:
                         found = True
         return board
 
-    def deal_raise_responder_nt_board(self, seat_index):
+    def raise_responder_nt_board(self, seat_index):
         """Return a hand where opener raises responder nt."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         loop = 1
         found = False
         board = None
         while not found:
             loop += 1
             openers_hand = get_hand([12, 19], SEMI_BALANCED_SHAPES)
             responders_hand = get_hand([6, 16], BALANCED_SHAPES, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands)
+            board = self.create_board(hands)
             board.dealer = SEATS[seat_index]
             auction = self._generate_auction_calls(board)
             if len(auction) >= 5:
                 openers_bid = auction[0]
                 responders_bid = auction[2]
                 openers_rebid = auction[4]
                 if (openers_bid.is_suit_call and
                         responders_bid.is_no_trumps and
                         openers_rebid.is_no_trumps):
                     if self._valid_overcalls(auction):
                         found = True
         return board
 
-    def deal_response_to_weak_two_board(self, seat_index):
+    def response_to_weak_two_board(self, seat_index):
         """Return a board requiring a response to weak two opening."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
             openers_hand = get_hand([6, 10], self.WEAK_TWO_SHAPES)
             responders_hand = get_hand([12, 19], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[partners_index])
+            board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
             auction = self._generate_auction_calls(board)
             openers_bid = auction[0]
             if openers_bid.level == 2:
                 if self._valid_overcalls(auction):
                     found = True
         return board
 
-    def deal_response_to_two_nt_board(self, seat_index):
+    def response_to_two_nt_board(self, seat_index):
         """Return a board requiring a response to two NT opening."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
             openers_hand = get_hand([20, 22], BALANCED_SHAPES)
             responders_hand = get_hand([0, 12], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[partners_index])
+            board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
             auction = self._generate_auction_calls(board)
             if self._valid_overcalls(auction):
                 found = True
         return board
 
-    def deal_response_to_two_clubs_board(self, seat_index):
+    def response_to_two_clubs_board(self, seat_index):
         """Return a board requiring a response to two clubs opening."""
-        get_hand = self.engine.get_hand_from_points_and_shape
+        get_hand = self.generate_hand
         found = False
         loop = 0
         board = None
         while not found:
             loop += 1
             openers_hand = get_hand([23, 30])
             responders_hand = get_hand([0, 12], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
-            board = self.engine.create_board_from_hands(hands, SEATS[partners_index])
+            board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
             auction = self._generate_auction_calls(board)
             if self._valid_overcalls(auction):
                 found = True
         return board
```

### Comparing `bfgdealer-0.0.3/bfgdealer.egg-info/PKG-INFO` & `bfgdealer-0.0.4/bfgdealer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.3
+Version: 0.0.4
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.4 05 May 2023
+
+1. Change set hands defn
+
+------
+
 Version 0.0.3 14 Mar 2023
 
 1. Improve condition checking on negative doubles
 
 ------
 
 Version 0.0.2 08 Mar 2023
```

### Comparing `bfgdealer-0.0.3/setup.py` & `bfgdealer-0.0.4/setup.py`

 * *Files identical despite different names*

