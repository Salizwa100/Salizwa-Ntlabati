# Salizwa-Ntlabati
# Assignment 1
import random

def play_game():
  # Define the options
  options = ["rock", "paper", "scissors]

  # Get user input
  user_options = input("Enter rock, paper, or scissors: ").lower()

  # Validate user input
  if user_options not in options:
        print("Invalid choice/ option! Please choose rock, paper, or scissors.")
        return

# Get computer's choice
  computer_choice = random.choice(choices)

# Display choices
  print(f"\nYou chose: {user_options}")
  print(f"The computer chose: {computer_choice}")

# Determine the winner
  if user_choice == computer_choice:
        print("It's a tie!")
    elif (user_options == "rock" and computer_choice == "scissors") or \
         (user_options == "paper" and computer_choice == "rock") or \
         (user_options == "scissors" and computer_choice == "paper"):
        print("You win!")
    else:
        print("Computer wins!")

# Play the game
if __name__ == "__main__":
    play_game()

