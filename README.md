# XOGAME
#### Video Demo: <https://youtu.be/HLwvX-GvXxE>
#### Description: 
In these file I going to explaining my project which is X-O_GAME
Fistful, why I choose this Idea because I think the purpose of project is implementing what we have learned in CS#50 course
so, I didnot take complex Idea to lose the gool of project and depend In myself only.
Now we are going to explain the code:
first, we import two libraries which are tkinter which help us to make a graphical user interface and this library is in our codespace we did not need to upload it and random library we also use it and it is in our codespace also 
to implement the project, we have to define somethings such as: 
next_turn: that will help us to transfer the turn from the first player two second one we use verity functions here:
global player that is help me which player click in the board first then
in line 6 we use if to tell me if the squares that is click was empty square because to make our game working we should not change the symbols during the game and if there is no winning yet then the second if to make who's click a first player and suppose the as randomly x-o and put it in the squares by the player click in the square 
the third if- function for if any player wins if no switch the turn to the second player we use the label in line 10 to know which player is play now 
elif- function in line 12 for: if the player wins show him as a winner by label fuction we use label to shown text in the window game in line 13 
the else in line 15 for if non-empty squares remains so no player can click then the we have tie game 
And for second player:
if to decide if the sequre is empty or not if the squares that is click was empty square and if there is no winning yet then the second if to make who's click a first player and suppose the as randomly x-o and put it in the squares by the player click in the square 
the third if- function for if any player wins if no switch the turn to the second player 
we use the label in line 10 to know which player is play now 
elif- function in line 12 for: if the player wins show him as a winner by label fuction we use label to shown text in the window game in line 13 
the else in line 15 for if non-empty squares remains so no player can click then the we have tie game 

 


Now we explain the check_winner:
where we use it to testing the difference win ways:
there are three possibilities horizontal wings and we express this by use for-loop 
we use row because it's horizontal and range 3 because we have 3 rows
the by if function to check if the symbol we write in 0-0 squares is it equal 0-1 squares and 0-2 squares if they equal each other and there is no empty squares on them then return True that mean we win!
and we use for-loop for the second possibility if the player chose the 1-0 and it was empty then in next turn 1-1 and also it is empty and last for 1-2 then the player will win [1-0, [1,1], and [1-2]] and we 
 use same for loop to implement it in last horizontal opportunity [2-0, [2,1], and [2-2]] and for all of them we add tremendous design by using config(bg="Green")
 we use col because it's vertical and range 3 because we have 3 COLs
the by if function to check if the symbol we write in 0-0 squares is it equal 1-0 squares and 2-0 squares if they equal each other and there is no empty squares on them then return True that mean we win!
and we use for-loop for the second possibility if the player chose the 0-1 and it was empty then in next turn 1-1 and also it is empty and last for 1-1 then the player will win [0-1, [1,1], and [2-1]] and we 
 use same for loop to implement it in last horizontal opportunity [0-2, [1,2], and [2-2]] and for all of them we add tremendous design by using config(bg="Green")

the last chance to win is in diagonals we have to diagonals 
so, we use if- function for that:
if the player select 0-0 square and it was empty then it is equal 1-1 square and equal 2-2 square then return to True that is mean we win and also the color of win is green 
second diagonal 
if the player select 0-2square and it was empty then it is equal 1-1square and equal 2,0 square then return to True that is mean we win and also the color of win is green 
0-2, 1-1, 2,0

Now we explain the check_empty_spaces:
the purpose for this is if this process equal false that is mean the is no empty squares and there is no one wins 
to change the color of all squares we made a loop for the ROWs and COLs and use config(bg="FFFF00") to get a yellow background color
then return tie
if all possibilities above no occur then we use else to return false and the check_empty_spaces is 3*3 matrix to build it we use for-loop 
and by if-function in each turn we subtract 1 from 9 until reach to 0 then return to zero else true 
For start_now_game we use it for:
choose random player to play and put the label refer to him then use it ro restart the match by convert the symbols with empty string and the orgioal color(#F0F0F0)
lastly 
we use window the shown up the game window and by window.title we choose the name of the file
then choose the competitors symbols 
the purpose of line 87 is choose randomly which player will start first
In line 94 we decide the location of label which is in middle
And in line 95 we use command for recall or use the strart_new_game 
last thon is window.mainloop() for to stay the widow shown 
Thanks for a cs50 team specially dived 
