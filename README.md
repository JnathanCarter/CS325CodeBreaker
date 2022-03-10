# CS325CodeBreaker
For your next project assignment, you will be implementing a simple game called "Codebreaker."  It is derived from the popular board game "Mastermind" from Invicta/Pressman, which itself is derived from other similar games (such as "Bulls and Cows") which have traditionally been played on paper.

In this game, the computer plays the role of the "Codemaker" and randomly generates a secret code.  The code takes the form of a sequence of four colored pegs, selected at random from six different colors: green, blue, red, yellow, brown, and orange.  The player's task as the "Codebreaker" is to guess all of the pegs of the code, in the correct sequence, in the least possible number of guesses.

In response to each of the player's guesses, the computer provides clues which can help the player to crack the code through a process of deduction.  The computer checks the code pegs guessed by the player, compares each of them to every one of the pegs in the secret code, and determines whether each code peg in the player's guess is of the correct color and is in the correct position (these are the "correct" pegs), or whether each code peg is of the correct color but is not in the correct position (these are the "misplaced" pegs).

With each guess, it counts the number of "correct" and "misplaced" code pegs, and displays these totals to the screen, alongside the player's guesses, in the form of key pegs: black key pegs indicate the number of "correct" code pegs, and white key pegs indicate the number of "misplaced" code pegs.  The code pegs in the player's guesses should be counted only once; that is, a code peg that is counted as "correct" must not also be matched with another peg of the same color and counted as "misplaced."  The total number of correct and misplaced pegs should never exceed the length of the code; if it does, your program is almost certainly counting the peg(s) twice.  The player can use this information to determine which code pegs need to be exchanged or replaced, until the player's guess exactly matches the secret code.  The computer then displays a message of congratulations, along with the total number of guesses it took the player to crack the code.

The attached archive contains a "how to play" guide in the form of a standalone Web page, adapted from The Playboy Winner's Guide to Board Games by Jon Freeman, which describes the rules and strategies of the game in more detail.  To better acquaint yourself with the game, please review this guide carefully before you begin writing your program for this assignment; you may find it helpful to "replay" the sample games shown there to test whether your program is producing the correct feedback.  This guide should be linked on the main Web page for your game, as shown in the example screenshot below, so that players can open it in a new browser tab or window simply by clicking the link.  The archive also contains a copy of the current jQuery library.

As we have done in our earlier assignments, create a new folder for this project called "Project2", and extract the files from the archive inside this folder.  To create the other files for this assignment, including the main Web page for your game and the JavaScript program file, refer back to your earlier work and to the examples given in the lecture notes as a starting point.  Your completed JavaScript program should be organized using objects and closure, as we have discussed in our earlier assignments.

The player should be presented with a drop-down selection of peg colors in an HTML form, one for each of the four slots of the code, as shown in the screenshot below.  When the player clicks "Submit," the selected code pegs should be compared to the secret code, as described above.  The results should be added to an HTML table below the form, with the row number, code pegs, and key pegs for each new guess placed at the top of the table.  To see an example of how to create the results table, study the sample games shown in the attached "how to play" guide; if you view the HTML source for this page, you will see how the samples have been formatted as HTML tables, and you can follow the same format in your program.  To create the pegs in your output as HTML characters, you can use the following HTML character entities:

&#x1F7E2;	🟢 (green)
&#x1F535;	🔵 (blue)
&#x1F534;	🔴 (red)
&#x1F7E1;	🟡 (yellow)
&#x1F7E4;	🟤 (brown)
&#x1F7E0;	🟠 (orange)
&#x26AB;	⚫ (black)
&#x26AA;	⚪ (white)
This project is worth 100 points toward the "Projects" portion of your grade and is due by the end of the day on Sunday, March 20th.  When you are finished, compress all of the files in your Web application to a ZIP archive, and submit the archive to Canvas.  The output of your completed program should resemble the following:

p2_complete.png
