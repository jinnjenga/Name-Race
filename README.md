# Name-Race
individual class project
# CS151 PROGRAMMING ASSIGNMENT #4

* 60  POINTS (10pts design, 50pts final)                                  			
* DESIGN DUE: 3/22/23
* FINAL DUE: 3/29/23

## PROBLEM:

You are designing a two-player game called The Name Race. In this game you have a set number of spots where a player can write their name. On a player's turn they roll a die, and if the spot associated with that number is empty, they write their name. Otherwise, they don't get to add a name that turn. Players continue taking turns until either a player quits, or all of the spots are filled. The winner of the game is the person who has filled the most spots with their name.

In this program, the user is one player, and the computer is the other player.

## PURPOSE OF THE ASSIGNMENT

The purpose of this assignment is to give you practice with

1. Input & output
2. Decision making
3. Looping
4. Function design and implementation
5. Error checking
6. Lists

## REQUIREMENTS ANALYSIS 

The first stage in your programming assignment is the requirements analysis stage.  You need to make sure you understand the below requirements for what needs to be included in your program.

You are creating a game for the user to play against the computer. The computer and the human player follow the same rules for the game. The coin flips and die rolls are all achieved via randomness in your program; no actual coins are flipped, and no actual dice are rolled.

For The Name Race, turn taking works a bit differently than in many games. Instead of alternating turns, a coin is flipped each time to determine who takes a turn. This rule means that one player may get multiple turns in a row, potentially achieving a win before the other play has a turn!

There are 6 spots to be filled. On a player's turn they roll a 6 sided die to determine which spot they have the opportunity to write their name in. However, they can only write their name there if it is empty! They cannot overwrite the other player's name, or re-write their name if it is already there.

The winner of a round is the player who has the most spots with their name in it at the end of the round. If both players have 3 spots filled, the round results in a tie. 

A human player can also give up after any turn. Before the game flips the coin to determine a turn, the user should be given a choice of whether another turn should be played or the game should end. 

### Winning the Game

Points are earned based on the outcome of a round; the first player to 10 points wins the game. At the end of a round, a tie results in each player earning 1 point; otherwise, the winner receives 5 points and the loser receives 0 points. If the human player chooses to quit, the computer player is awarded 10 points. The first player to earn at least 10 points wins the game, and the program ends at that time.

### Iterative development

The best way to design a program is to use iterative development. This means get it working in pieces. For instance, figure out how to represent the game and play with only 1 human player, who plays until they've filled all spots with their name. Only once that works try to add in a computer player. Create a game that ends as soon as someone wins a round; only once that works, worry about how to do multiple rounds with points. Working on your program this way will make it easier to test and fix errors as you work.

### General design requirements

Your game must explain the rules to the user at the start. We have learned how to do quite a bit of formatting at this point in the semester -- try to use some of it.

Your game should output the state of the 6 spots after every turn, so the user knows what is happening. Your game should also output the results of coin flips or die rolls, and what is done by the computer player. The user should be able to understand the game.

Be sure to do error checking on the user's input for when you ask them if they want to quit the game.

## DESIGN

The second stage is to design your solution based on the requirements:

1. Determine the tasks being accomplished in your program. Each of these should be a function. If you find yourself writing the same steps in many places, that is usually a good sign that those steps should be in their own function. A group of steps that are highly related to each other also should be a function.
2. Write an algorithm for each function. This algorithm includes parameters, calculations, and returned values. No code other than import statements and the call to main should exist outside of a function.
3. Make the main part of your program be in a “main” function. The main function never takes parameters, and does not return anything. The main function will call most of your other functions.
4. Double check that you included all of the requirements.


### DESIGN SUBMISSION: 

Submit to GitHub in PA4 repository: the algorithm for your game in designInitial.txt. Remember to note the name, parameters, return value, and algorithm for every function.

*Remember to double check on github.com that your file pushed. If it didn't, you need to push it. Your instructor can only see what is on github.com, not what is only on your computer.*

Your algorithm should follow the requirements of an algorithm, contain all of the requirements, and include your entire program. Everything should be planned out. There should not be any code.

## PROGRAMMING STEPS

After your design is complete and correct, it's time to start programming and then testing:

* Fix design issues: If there were issues with your design, either not meeting requirements or in the format, fix that before you start writing your code.
* Implementation: Write your program following the requirements and based on your design.
  * Follow good usability/HCI principles in your input and output (make it clear the type of input you are asking for)
  * Follow good use of functions
  * Remember to define functions before they are used (so if function A calls function B, you need to define function B first in your program)
  * Remember to state the purpose of the program
  * Remember to have a main function, and to call it.
* Testing: Make sure it works correctly; give it sample input, and check that the output is correct. You should be testing as your work, following iterative development. Only work on coding a new part of the game after you got a simpler part working.


## EXTRA CREDIT (only if everything else works)

If you choose to do extra credit, it must be submitted in a separate file with "extraCredit" in the file name. Your extra credit program is also The Name Race, but with a key difference: the user can choose the number of spots that exist in the game board. You must do error checking on this input to ensure it is valid before you use it, to make sure your program does not crash. Then the game should run the same way as before, just with the size of board specified by the user.


## ASSIGNMENT REMINDERS

Follow the programming assignment requirements document for comments, formatting, etc.

## REFLECTION

Write a short reflection about the programming assignment in reflection.txt: what did you learn, what would you do differently next time, what was difficult?  This should be no more than a page.

## FINAL SUBMISSION

1. To GitHub:  
    1. Your .py file  
    2. Your extra credit .py file if you did the extra credit (make sure "extraCredit" is in the filename)  
    3. Your final algorithm, including the changes you made based on the design feedback, in designFinal.txt
    4. Your reflection of the programming assignment in reflection.txt.

***Remember to double check on github.com that your files pushed. If they didn’t, you need to push them. Your instructor can only see what is on github.com, not what is only on your computer.***

