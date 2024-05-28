# Comparing `tmp/STTT-0.8.tar.gz` & `tmp/sttt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STTT-0.8.tar", last modified: Thu Nov 16 18:50:47 2023, max compression
+gzip compressed data, was "sttt-1.0.0.tar", max compression
```

## Comparing `STTT-0.8.tar` & `sttt-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-11-16 18:50:47.797759 STTT-0.8/
--rw-rw-rw-   0        0        0     1095 2023-11-16 16:28:41.000000 STTT-0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3759 2023-11-16 18:50:47.796370 STTT-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-11-16 18:44:26.000000 STTT-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-16 18:50:47.793804 STTT-0.8/STTT.egg-info/
--rw-rw-rw-   0        0        0     3759 2023-11-16 18:50:47.000000 STTT-0.8/STTT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-11-16 18:50:47.000000 STTT-0.8/STTT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-16 18:50:47.000000 STTT-0.8/STTT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-11-16 18:50:47.000000 STTT-0.8/STTT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-11-16 18:50:47.000000 STTT-0.8/STTT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-16 18:50:47.797759 STTT-0.8/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-11-16 18:44:31.000000 STTT-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-16 18:50:47.795057 STTT-0.8/sttt/
--rw-rw-rw-   0        0        0        0 2023-11-16 18:44:31.000000 STTT-0.8/sttt/__init__.py
--rw-rw-rw-   0        0        0     4769 2023-11-16 18:44:31.000000 STTT-0.8/sttt/__main__.py
+-rw-r--r--   0        0        0     1095 2023-11-16 16:28:41.890256 sttt-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      568 2024-05-28 11:58:10.018882 sttt-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 2023-11-16 18:44:26.418310 sttt-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-11-16 18:44:31.635839 sttt-1.0.0/sttt/__init__.py
+-rw-r--r--   0        0        0     5573 2024-05-28 10:42:52.607644 sttt-1.0.0/sttt/__main__.py
+-rw-r--r--   0        0        0     3218 2023-11-16 18:44:31.635839 sttt-1.0.0/sttt/README.md
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 sttt-1.0.0/PKG-INFO
```

### Comparing `STTT-0.8/LICENSE.txt` & `sttt-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `STTT-0.8/PKG-INFO` & `sttt-1.0.0/sttt/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: STTT
-Version: 0.8
-Summary: CLI implementation of the game "Super Tic Tac Toe" written in python
-Home-page: https://github.com/Zamiul-rashid/Super-Tic-Tac-Toe
-Author: Zamiul, Proyas
-Author-email: zamiulrashid1@gmail.com,abyashrirproyas@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Super Tic Tac Toe Console Game
 
 This Python console-based game is an implementation of the classic Tic Tac Toe with an added twist - Super Tic Tac Toe. The game is played on a larger board consisting of nine smaller Tic Tac Toe boards arranged in a 3x3 grid.
 
 ## Rules of the Game
 
 1. **Board Layout**:
```

### Comparing `STTT-0.8/README.md` & `sttt-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `STTT-0.8/sttt/__main__.py` & `sttt-1.0.0/sttt/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-
+"""...Fix input bug..."""
 def cls():
     os.system('cls' if os.name in ('nt', 'dos') else 'clear')
 
 disabled = '\033[02m'
 highlight_color = '\033[47m'+'\033[30m'
 X_color = '\033[01m'+'\033[93m'
 Y_color = '\033[01m'+'\033[36m'
@@ -43,18 +43,18 @@
                 print("---|---|---")
         else:
             return " │ ".join(self.board[lineno])
     '''Checking for winner in the smaller board for each player'''
     def checkWin(self):
         wins = [[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]]
         for win in wins:
-            if self.board[win[0]//3][win[0]%3] == self.board[win[1]//3][win[1]%3] == self.board[win[2]//3][win[2]%3]:
-                return self.board[win[1]//3][win[1]%3]    
+            if self.board[win[0]//3][win[0]%3] == self.board[win[1]//3][win[1]%3] == self.board[win[2]//3][win[2]%3]:#Comparing the 
+                return self.board[win[1]//3][win[1]%3]                                          # elements of the board to check for winner
         return None
-        
+
     def play (self,num,C_P):
         self.board[num//3][num%3]=C_P
         self.won = self.checkWin() 
                      
                 
         
 class super_tic_tac_toe:
@@ -102,39 +102,55 @@
         wins = [[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]]
         for win in wins:
             if self.sboard[win[0]//3][win[0]%3].won == self.sboard[win[1]//3][win[1]%3].won == self.sboard[win[2]//3][win[2]%3].won:
                 return self.sboard[win[1]//3][win[1]%3].won    
         return None
 
 def playgame():
+    x = 1
     player = "X" 
     boardno = 4
     Tic = super_tic_tac_toe()
-
+    ele_check = tic_tac_toe()
     while True:
         cls()
         logoDisplay()
         Tic.showboard(boardno)
         print()
         if Tic.checkWin() != None :
             """Print winner"""
             print(f"{Tic.checkWin()} is the winner !!!")
             break
         while Tic.get_Board(boardno).won != None :
             boardno = int(input(f"Please enter a board other then {boardno+1} : "))-1
-
-        
-        Inp = int(input(f"{(X_color if player == 'X' else Y_color)+player} Input : {RESET}"))-1
-     
+        #The input peradox problem
+        while True :
+            try:
+                Inp = int(input(f"{(X_color if player == 'X' else Y_color)+player} Input : {RESET}"))-1
+                if Inp not in range(9):
+                    print(f"{Inp+1} is not on the board")
+                    continue
+                if Tic.get_Board(boardno).board[Inp//3][Inp%3] in ["X","O"]:
+                    print("The box is already filled")
+                    continue
+                break
+            except KeyboardInterrupt:
+                exit()
+            except:
+                print(f"Invalid input!")
+                continue 
+        # the above loop will force the user to enter a valid input.INPUT PARADOX SOLVED 
+              
+         
         Tic.get_Board(boardno).play(Inp,player)
         
         boardno = Inp
         player = "O" if player == "X" else "X"
 
-# if __name__ == "__main__":
-#     playgame()
+if __name__ == "__main__":
+    
+    playgame()
 
     
 
 # Testing sequence
-# [(0,0),(6,0),(2,0),(4,1),(0,"b2",4),(4,2),(6,4),(8,0),("b8",4,"b2",8),(6,8),(2,"Winner!!")]    
-
+# [(0,0),(6,0),(2,0),(4,1),(0,"b2",4),(4,2),(6,4),(8,0),("b8",4,"b2",8),(6,8),(2,"Winner!!")]
```

