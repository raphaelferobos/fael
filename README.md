import random

def play_game():
    number_to_grab = random.randint(1, 10)
    guess = None
    attempts = 0

    while guess != number_to_guess:
        guess = int(input("Guess the number to grab between 1 and 10: "))
        attempts += 1
        if guess < number_to_guess:
            print("Too low! Try again.")
        elif guess > number_to_guess:
            print("Too high! Try again.")
    
    print(f"Congratulations! You grabbed the number {number_to_guess} in {attempts} attempts.")

if __name__ == "__main__":
    play_game()
