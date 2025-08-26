# python
Number Guessing Game in Python
A simple command-line guessing game where the user tries to guess a randomly generated number between 1 and 100.
________________________________________
Project Structure
guessing-game/
├── guessing_game.py
├── README.md
└── LICENSE
________________________________________
guessing_game.py
Python
import random
def guessing_game():
    number_to_guess = random.randint(1, 100)
    tries = 0
    while True:
        user_guess = input("Guess a number between 1 and 100: ")
        if not user_guess.isdigit():
            print("Invalid input. Please enter a whole number.")
            continue
        user_guess = int(user_guess)
        tries += 1
        if user_guess == number_to_guess:
            print(f"You are right, great job! It took you {tries} tries.")
            break
        elif user_guess < number_to_guess:
            print("Your guess is low, try again!")
        else:
            print("Your guess is high, try again!")
if __name__ == "__main__":
    guessing_game()
________________________________________
README.md
Markdown
# Number Guessing Game in Python
A simple number guessing game where the user has to guess a randomly generated number between 1 and 100.
## How to Play
- The system generates a random number between 1 and 100.
- Enter your guess (a number between 1 and 100).
- The program will tell you if your guess is too low, too high, or correct.
- The game ends when you guess the correct number.
## How to Run
1. Make sure you have Python installed.
2. Run the game with:
python guessing_game.py
## Example Output
Guess a number between 1 and 100: 50
Your guess is low, try again!
Guess a number between 1 and 100: 75
Your guess is high, try again!
Guess a number between 1 and 100: 63
You are right, great job! It took you 3 tries.

