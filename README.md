# Salizwa-Ntlabati
Software Engineering 

import random
# Assignment 1 - Rock-Paper-Scissors

# Get computer's choice
def get_computer_choice():
    choices = ['R','P','S']
    return random.choice(choices)

# Get users choice
def get_user_choice():
    while True:
        user_input = input("Enter R for Rock, P for Paper, or S for Scissors: ")
        if user_input in ['R','P','S']:
            return user_input
        else:
            print("Invalid choice. Please choose R, P, or S.")

# Define the Rules
def determine_winner(user_choice, computer_choice):
    if user_choice == computer_choice:
        return "It's a tie!"
    elif (user_choice == 'R' and computer_choice == 'S') or \
         (user_choice == 'P' and computer_choice == 'R') or \
         (user_choice == 'S' and computer_choice == 'P'):
        return "You win!"
    else:
        return "You lose!"

def play_game():
    print("Welcome to Rock, Paper, Scissors!")
    user_choice = get_user_choice()
    computer_choice = get_computer_choice()

  print(f"You chose {user_choice}.")
  print(f"The computer chose {computer_choice}.")

  result = determine_winner(user_choice, computer_choice)
    print(result)

if __name__ == "__main__":
    play_game()
