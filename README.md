# Number-Game
1-100
import random

def number_game():
    number_to_guess = random.randint(1, 100)
    guess = None
    attempts = 0

    while guess != number_to_guess:
        guess = int(input("Guess a number between 1 and 100: "))
        attempts += 1

        if guess < number_to_guess:
            print("Higher!")
        elif guess > number_to_guess:
            print("Lower!")
        else:
            print(f"Congratulations! You've guessed the number in {attempts} attempts.")

if __name__ == "__main__":
    number_game()
