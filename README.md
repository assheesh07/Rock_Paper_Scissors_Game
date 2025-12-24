# Rock_Paper_Scissors_Game
a simple Python Rock, Paper, Scissors game you can use, it takes user input, makes the computer choose randomly, and tells you who wins

Code: 

import random

options = ["rock", "paper", "scissors"]

while True:
    user_choice = input("Enter rock, paper, or scissors: ")

    computer_choice = random.choice(options)

    print("You chose:", user_choice)
    print("Computer chose:", computer_choice)

    if user_choice not in options:
        print("Invalid choice — please try again!")
        continue

    if (user_choice == computer_choice):
        print("It's a tie!")
    elif (user_choice == "rock" and computer_choice == "scissors") or \
         (user_choice == "paper" and computer_choice == "rock") or \
         (user_choice == "scissors" and computer_choice == "paper"):
        print("You win!")
    else:
        print("You lose!")

    print() 
