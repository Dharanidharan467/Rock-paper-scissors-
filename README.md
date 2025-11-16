# Rock-paper-scissors-
import random

def play():
    print("Welcome to Rock, Paper, Scissors!")
    print("Choices: rock, paper, or scissors")

    user = input("Enter your choice: ").lower()
    choices = ["rock", "paper", "scissors"]
    computer = random.choice(choices)

    print(f"\nYou chose: {user}")
    print(f"Computer chose: {computer}\n")

    if user not in choices:
        print("Invalid choice! Please choose rock, paper, or scissors.")
        return

    if user == computer:
        print("It's a tie!")

    elif (user == "rock" and computer == "scissors") or \
         (user == "paper" and computer == "rock") or \
         (user == "scissors" and computer == "paper"):
        print("You win! 🎉")

    else:
        print("You lose! 😢")


# Run the game
play()
