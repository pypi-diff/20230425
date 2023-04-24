# Comparing `tmp/chessmaker-0.4.1.tar.gz` & `tmp/chessmaker-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.4.1.tar", max compression
+gzip compressed data, was "chessmaker-0.4.2.tar", max compression
```

## Comparing `chessmaker-0.4.1.tar` & `chessmaker-0.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.4.1/chessmaker/__init__.py
--rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.4.1/chessmaker/chess/__init__.py
--rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.4.1/chessmaker/chess/base/__init__.py
--rw-r--r--   0        0        0     6811 2023-04-22 18:15:44.473745 chessmaker-0.4.1/chessmaker/chess/base/board.py
--rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.4.1/chessmaker/chess/base/game.py
--rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.4.1/chessmaker/chess/base/move_option.py
--rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.4.1/chessmaker/chess/base/piece.py
--rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.4.1/chessmaker/chess/base/player.py
--rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.4.1/chessmaker/chess/base/position.py
--rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.4.1/chessmaker/chess/base/rule.py
--rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.4.1/chessmaker/chess/base/square.py
--rw-r--r--   0        0        0     5151 2023-04-22 18:15:44.474745 chessmaker-0.4.1/chessmaker/chess/game_factory.py
--rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.4.1/chessmaker/chess/piece_utils.py
--rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.4.1/chessmaker/chess/pieces/__init__.py
--rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.4.1/chessmaker/chess/pieces/bishop.py
--rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.4.1/chessmaker/chess/pieces/king.py
--rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.4.1/chessmaker/chess/pieces/knight.py
--rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.4.1/chessmaker/chess/pieces/knook/__init__.py
--rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knook.py
--rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable.py
--rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.4.1/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.4.1/chessmaker/chess/pieces/pawn.py
--rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.4.1/chessmaker/chess/pieces/queen.py
--rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.4.1/chessmaker/chess/pieces/rook.py
--rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.4.1/chessmaker/chess/results/__init__.py
--rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.4.1/chessmaker/chess/results/capture_all_pieces_to_win.py
--rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.4.1/chessmaker/chess/results/checkmate.py
--rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.4.1/chessmaker/chess/results/double_check_to_win.py
--rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.4.1/chessmaker/chess/results/no_captures_or_pawn_moves.py
--rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.4.1/chessmaker/chess/results/repetition.py
--rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.4.1/chessmaker/chess/results/stalemate.py
--rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.4.1/chessmaker/chess/results/standard_result.py
--rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.4.1/chessmaker/chess/rules/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.4.1/chessmaker/chess/rules/beta_decay.py
--rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.4.1/chessmaker/chess/rules/forced_en_passant.py
--rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.4.1/chessmaker/chess/rules/il_vaticano.py
--rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.4.1/chessmaker/chess/rules/king_cant_move_to_c2.py
--rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.4.1/chessmaker/chess/rules/knight_boosting.py
--rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.4.1/chessmaker/chess/rules/la_bastarda.py
--rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.4.1/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.4.1/chessmaker/chess/rules/siberian_swipe.py
--rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.4.1/chessmaker/clients/__init__.py
--rw-r--r--   0        0        0    18171 2023-04-22 18:29:36.629482 chessmaker-0.4.1/chessmaker/clients/pywebio_ui.py
--rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.4.1/chessmaker/cloneable.py
--rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.4.1/chessmaker/events/__init__.py
--rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.4.1/chessmaker/events/event.py
--rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.4.1/chessmaker/events/event_priority.py
--rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.4.1/chessmaker/events/event_publisher.py
--rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.4.1/LICENSE
--rw-r--r--   0        0        0     1098 2023-04-22 18:29:36.624482 chessmaker-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.4.1/README.md
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.4.2/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.4.2/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.4.2/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6811 2023-04-22 18:15:44.473745 chessmaker-0.4.2/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.4.2/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.4.2/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.4.2/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.4.2/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.4.2/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.4.2/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.4.2/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5281 2023-04-22 20:33:13.515140 chessmaker-0.4.2/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.4.2/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.4.2/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.4.2/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     7173 2023-04-22 22:31:36.777549 chessmaker-0.4.2/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.4.2/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.4.2/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.4.2/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.4.2/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.4.2/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.4.2/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      331 2023-04-22 19:21:15.298254 chessmaker-0.4.2/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.4.2/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.4.2/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.4.2/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.4.2/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      961 2023-04-24 20:44:49.437636 chessmaker-0.4.2/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.4.2/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      680 2023-04-22 19:21:15.309254 chessmaker-0.4.2/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.4.2/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.4.2/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.4.2/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.4.2/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.4.2/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.4.2/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.4.2/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.4.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.4.2/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.4.2/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    18218 2023-04-24 20:46:07.131795 chessmaker-0.4.2/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.4.2/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.4.2/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.4.2/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.4.2/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.4.2/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1098 2023-04-22 20:38:50.134595 chessmaker-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.4.2/README.md
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.4.2/PKG-INFO
```

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/__init__.py` & `chessmaker-0.4.2/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/board.py` & `chessmaker-0.4.2/chessmaker/chess/base/board.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/game.py` & `chessmaker-0.4.2/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/piece.py` & `chessmaker-0.4.2/chessmaker/chess/base/piece.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/player.py` & `chessmaker-0.4.2/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/rule.py` & `chessmaker-0.4.2/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/base/square.py` & `chessmaker-0.4.2/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/game_factory.py` & `chessmaker-0.4.2/chessmaker/chess/game_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,19 +109,23 @@
         result_functions.insert(0, results.capture_all_pieces_to_win)
     else:
         result_functions.insert(0, checkmate)
 
     if double_check_to_win:
         result_functions.insert(0, results.double_check_to_win)
 
-    def get_result(board: Board) -> str:
-        for result_function in result_functions:
-            result = result_function(board)
-            if result:
-                return result
+    class GetResult:
+        def __init__(self):
+            self.result_functions = result_functions
+
+        def __call__(self, board: Board):
+            for result_function in self.result_functions:
+                result = result_function(board)
+                if result:
+                    return result
 
     game = Game(
         board=Board(
             squares=[
                 [Square(piece_row[i](black)) for i in range(8)],
                 [Square(_pawn(black)) for _ in range(8)],
                 _empty_line(8),
@@ -131,11 +135,11 @@
                 [Square(_pawn(white)) for _ in range(8)],
                 [Square(piece_row[i](white)) for i in range(8)],
             ],
             players=[white, black],
             turn_iterator=turn_iterator,
             rules=rules,
         ),
-        get_result=get_result,
+        get_result=GetResult(),
     )
 
     return game
```

### Comparing `chessmaker-0.4.1/chessmaker/chess/piece_utils.py` & `chessmaker-0.4.2/chessmaker/chess/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/king.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/king.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import contextmanager
 from dataclasses import dataclass
 from functools import partial
 from typing import Iterable
 
 from chessmaker.chess.base.board import AfterNewPieceEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, BeforeMoveEvent, BeforeGetMoveOptionsEvent
@@ -72,16 +73,27 @@
             move_options = piece.get_move_options()
 
             for move_option in move_options:
                 if self.position in move_option.captures:
                     return True
         return False
 
+    @contextmanager
+    def _make_kings_attackable(self):
+        for piece in self.board.get_pieces():
+            if isinstance(piece, King):
+                piece._attackable = True
+        yield
+        for piece in self.board.get_pieces():
+            if isinstance(piece, King):
+                piece._attackable = False
+
     def _is_attacked_after_move(self, piece: Piece, move_option: MoveOption) -> bool:
-        board_clone = self.board.clone()
+        with self._make_kings_attackable():
+            board_clone = self.board.clone()
         self_clone = board_clone[self.position].piece
         piece_clone = board_clone[piece.position].piece
         piece_clone.move(move_option)
         return self_clone.is_attacked()
 
     def _on_before_get_move_options(self, event: BeforeGetMoveOptionsEvent):
         if event.piece.player != self.player:
@@ -159,9 +171,8 @@
             rook_source.piece = None
             rook.moved = True
 
             self.publish(AfterCastleEvent(self, rook))
         self._moved = True
 
     def clone(self):
-        # TODO: What if someone else clones the king?
-        return King(self.player, self._moved, attackable=True, castling_directions=self._castling_directions)
+        return King(self.player, self._moved, attackable=self._attackable, castling_directions=self._castling_directions)
```

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/knight.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/queen.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/pieces/rook.py` & `chessmaker-0.4.2/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/results/checkmate.py` & `chessmaker-0.4.2/chessmaker/chess/results/checkmate.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/results/double_check_to_win.py` & `chessmaker-0.4.2/chessmaker/chess/results/double_check_to_win.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/results/no_captures_or_pawn_moves.py` & `chessmaker-0.4.2/chessmaker/chess/results/no_captures_or_pawn_moves.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/results/repetition.py` & `chessmaker-0.4.2/chessmaker/chess/results/repetition.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,10 +16,10 @@
                 if square is None:
                     position_hash += "None"
                 elif square.piece is None:
                     position_hash += "Empty"
                 else:
                     position_hash += square.piece.__class__.__name__ + square.piece.player._id
 
-        self.positions[position_hash] += 1
+        self.positions[position_hash] = self.positions.get(position_hash, 0) + 1
         if self.positions[position_hash] >= self.needed_repetitions:
             return "Repetition - Draw"
```

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.4.2/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.4.2/chessmaker/chess/rules/forced_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.4.2/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/king_cant_move_to_c2.py` & `chessmaker-0.4.2/chessmaker/chess/rules/king_cant_move_to_c2.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.4.2/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/la_bastarda.py` & `chessmaker-0.4.2/chessmaker/chess/rules/la_bastarda.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.4.2/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.4.2/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.4.2/chessmaker/clients/pywebio_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
 def on_game_end(event: AfterGameEndEvent):
     popup("Game Over", event.result)
 
 
 def share_position():
     board = session_data.game.board.clone()
-    get_result = session_data.game._get_result
+    get_result = deepcopy(session_data.game._get_result)
     options = client_games[session_data.game_id].options
     piece_urls = client_games[session_data.game_id].piece_urls
 
     position_id = str(uuid4())
     shared_positions[position_id] = SharedPosition(board, get_result, options, piece_urls)
 
     run_js("navigator.clipboard.writeText(window.location.href.split('?')[0] + '?position_id=' + position_id);",
@@ -406,15 +406,15 @@
                     radio("Mode", ["Singleplayer", "Multiplayer (Private)", "Multiplayer (Public)"], name="mode",
                           value="Singleplayer"),
                     actions("-", [
                         {"label": "Create", "value": "create"},
                     ], name="action"),
                 ])
                 shared_position = shared_positions[get_query("position_id")]
-                new_game(lambda **_: Game(shared_position.board, shared_position.get_result),
+                new_game(lambda **_: Game(shared_position.board.clone(), deepcopy(shared_position.get_result)),
                             shared_position.options, form_result["mode"], piece_urls)
             return
 
         form_result = input_group("New Game", [
             radio("Mode", ["Singleplayer", "Multiplayer (Private)", "Multiplayer (Public)"], name="mode",
                   value="Singleplayer"),
             checkbox(
@@ -445,9 +445,9 @@
 if __name__ == "__main__":
     start_pywebio_chess_server(
         create_game,
         supported_options=["chess960", "knooks", "forced_en_passant", "knight_boosting", "omnipotent_f6_pawn",
                            "siberian_swipe", "il_vaticano", "beta_decay", "la_bastarda", "king_cant_move_to_c2",
                            "vertical_castling", "double_check_to_win", "capture_all_pieces_to_win"],
         piece_urls=PIECE_URLS | {"Knook": ["https://i.imgur.com/UiWcdEb.png", "https://i.imgur.com/g7xTVts.png"]}
-        , debug=True
+        ,remote_access=True, debug=True
     )
```

### Comparing `chessmaker-0.4.1/chessmaker/events/event_publisher.py` & `chessmaker-0.4.2/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/LICENSE` & `chessmaker-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/pyproject.toml` & `chessmaker-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chessmaker"
-version = "0.4.1"
+version = "0.4.2"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = ["WolfDWyc <yoavwolfdw@gmail.com>",]
 license = "AGPL-3.0-or-later"
 classifiers = [
 "License :: OSI Approved :: GNU Affero General Public License v3",
 "Programming Language :: Python",
```

### Comparing `chessmaker-0.4.1/README.md` & `chessmaker-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.1/PKG-INFO` & `chessmaker-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.4.1
+Version: 0.4.2
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 License: AGPL-3.0-or-later
 Keywords: chess
 Author: WolfDWyc
 Author-email: yoavwolfdw@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

