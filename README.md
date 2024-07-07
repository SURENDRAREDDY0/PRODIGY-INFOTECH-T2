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


import java.util.Scanner;

public class numbergame
{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = 1 + (int)(100 * Math.random());
        int t = 5; // t = trials
        int i, g; // g = guess
        System.out.println("A number is chosen between 1 to 100");
        System.out.println("Guess the number within 5 trials");

        for (i = 0; i < t; i++) {
            System.out.println("Guess the number:");
            g = sc.nextInt();
            if (num == g) {
                System.out.println("Well done buddy, you guessed the number!");
                break;
            } else if (num > g && i != t - 1) {
                System.out.println("The number is greater than " + g);
            } else if (num < g && i != t - 1) {
                System.out.println("The number is smaller than " + g);
            }
        }

        if (i == t) {
            System.out.println("You have exhausted " + t + " trials.");
            System.out.println("The number was " + num);
            System.out.println("Play again\nBetter luck next time!");
        }
    }
}
