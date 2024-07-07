# PRODIGY-INFOTECH-T2
Create a Gussing Game
Initialization:

Scanner is used to read input from the user.
Random is used to generate a random number (secretNumber) between 1 and 100 inclusive.
Game Setup:

The game starts with a welcome message and instructions.
secretNumber is the number that the player needs to guess.
Game Loop:

The game continues in a loop (while (!hasGuessed)) until hasGuessed becomes true.
Inside the loop, the player is prompted to enter a guess.
The guess is compared to secretNumber:
If the guess is lower than secretNumber, a message is printed indicating it's too low.
If the guess is higher than secretNumber, a message is printed indicating it's too high.
If the guess equals secretNumber, a congratulatory message is printed, the number of attempts is displayed, and hasGuessed is set to true to exit the loop.
End of Game:

Once the player guesses the correct number, the game ends, and the Scanner is closed.
How to Play:
Run the program.
The computer will choose a random number between 1 and 100.
Enter your guess when prompted.
Based on your guess, the program will tell you if the number is too high or too low.
Keep guessing until you correctly guess the number.
After guessing correctly, the program will tell you how many attempts it took.
This game provides a fun and interactive way to practice conditional statements (if, else if, else) and loops (while) in Java.
