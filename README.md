# cst426TicTacToe

This project was a bit of a challenge compared to the first one. I thought I was going crazy when my work partner Freddie and I couldn't get anything to display, so I was happy to find out there was just a bug preventing the starting windows from rendering. As with last time, starting early and working together is the only way we were able to get through each method. It was a little fun to learn the ins and outs of how each method is arranged, but I admit I am still very weak with my C++ skills. I do not feel like I could write a game like this from scratch yet, but maybe this will prove to be good practice to get there, I am feeling a lot more confident than I did a month ago with all this. Writing C++ will continue until morale improves. 


addendum for negamax AI: 
Added methods for a negamax AI player that will iterate through all possible game states and should always result in a draw. 
https://en.wikipedia.org/wiki/Negamax 

The AI surveys all the avaliable squeares for an empty square, it temporarily puts a human player ther and then calls negamax and the best score is chosen for the AI's move. 

Negamax works by checking to see if it has completed a line and if so it returns -10 because any win on the board must have been by the previous player which means this must be a terminal state.  Once the board is full it returns 0. Otherwise it tries every empty square for the current player and recurses with roles flipped then negates the child's value and takes the maximum. Wins evaluate to +10 for the AI and losses -10. no depth cutoff means it searches all possiblities. 


