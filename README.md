NUMBER GUESSING GAME......

1. Random Number Generation
-> The program uses the rand() function to generate a random number. However, rand() alone is not truly random because it produces the same sequence of numbers each time the program runs unless it's "seeded" with a 
   different starting point.
-> srand(time(0)); is used to seed the random number generator with the current time (from time(0)), ensuring a different random number is generated every time you run the program.
-> rand() % 100 + 1 generates a random number between 1 and 100:
-> rand() % 100 generates numbers from 0 to 99, and by adding 1, the range becomes 1 to 100.
2. User Interaction
-> The program welcomes the user and asks them to guess a number between 1 and 100.
-> The user is prompted to enter their guess using cin.
3. Feedback on Guesses
-> After each guess, the program compares the user's input to the randomly generated number:
-> If the guess is too high (greater than the random number), the program responds with "Too high! Try again."
-> If the guess is too low (less than the random number), the program responds with "Too low! Try again."
-> If the guess is correct, the program responds with "Congratulations! You guessed the number correctly!" and ends the loop.
4. Looping Until the Correct Guess
-> The program uses a while loop to repeatedly ask for guesses until the user guesses the correct number. The loop condition is while (guess != randomNumber), which keeps the game running as long as the guess is 
   incorrect.
5. Ending the Game
-> Once the user guesses the correct number, the game congratulates the user and exits the loop, ending the program.
