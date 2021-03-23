# Lab-04
Brodie Fogarty - bfog012
Update this README to include your team name and team members. Don't forget to record all your answers to lab 04 here.

List three data types used in this program.
    Answer - interger, String, List
    
List any value variables or reference variables in this program.
    answer- i,dupeBoard,
    
Give an example of a sequence in this program.

-  return ((bo[7] == le and bo[8] == le and bo[9] == le) or # across the top
 (bo[4] == le and bo[5] == le and bo[6] == le) or # across the middle
 (bo[1] == le and bo[2] == le and bo[3] == le) or # across the bottom
 (bo[7] == le and bo[4] == le and bo[1] == le) or # down the left side
 (bo[8] == le and bo[5] == le and bo[2] == le) or # down the middle
 (bo[9] == le and bo[6] == le and bo[3] == le) or # down the right side
 (bo[7] == le and bo[5] == le and bo[3] == le) or # diagonal
 (bo[9] == le and bo[5] == le and bo[1] == le)) # diagonal
 
Give an example of a condition in this program.
   answer -if letter == 'X':
  return ['X', 'O']
  
Give an example of an iteration in this program.
    Answer-  while not (letter == 'X' or letter == 'O'):
              print('Do you want to be X or O?')
              letter = input().upper()
              
Give an example of a list or collection in this program. What is saved in the list / collection?

Answer- def chooseRandomMoveFromList(board, movesList):
 
 possibleMoves = []
 for i in movesList:
  if isSpaceFree(board, i):
   possibleMoves.append(i)
   
Give an example of a function that has at least one parameter in this program. And, briefly explain what the function is trying to achieve.

 def drawBoard(board):
   print('   |   |')
 print(' ' + board[7] + ' | ' + board[8] + ' | ' + board[9])
 print('   |   |')
 print('-----------')
 print('   |   |')
 print(' ' + board[4] + ' | ' + board[5] + ' | ' + board[6])
 print('   |   |')
 print('-----------')
 print('   |   |')
 print(' ' + board[1] + ' | ' + board[2] + ' | ' + board[3])
 print('   |   |')
 
 Where the function is trying to create the plate for the game
 
How does the program determine who wins the game? List the functions that the program use to determine the winner.

def isWinner(bo, le):

 return ((bo[7] == le and bo[8] == le and bo[9] == le) or # across the top
 (bo[4] == le and bo[5] == le and bo[6] == le) or # across the middle
 (bo[1] == le and bo[2] == le and bo[3] == le) or # across the bottom
 (bo[7] == le and bo[4] == le and bo[1] == le) or # down the left side
 (bo[8] == le and bo[5] == le and bo[2] == le) or # down the middle
 (bo[9] == le and bo[6] == le and bo[3] == le) or # down the right side
 (bo[7] == le and bo[5] == le and bo[3] == le) or # diagonal
 (bo[9] == le and bo[5] == le and bo[1] == le)) # diagonal

If the code on line 165 is changed from break to gameIsPlaying = False, will this change the behaviour of the program?
                    
                    No it doesnt change the behaviour because having gameIsPlaying = False breaks the loop.
What does while True: do in this program?
                    - Starts the game



 

