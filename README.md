# ergis
import random

choices = ["rock","paper","scissors"]

computer = random.choice(choices)
player = None

while player not in choices:
    player = input("rock , paper,scissors?: ").lower()
if player == computer:
    print("computer", computer)
    print("player", player)
    print("Tie")
elif player == "rock":
    if computer == "paper":
        print("computer", computer)
        print("player", player)
        print("You lose,sucker")
    if computer == "scissors":
        print("computer", computer)
        print("player", player)
        print("You win")
elif player == "paper":
    if computer == "rock":
        print("computer", computer)
        print("player", player)
        print("You win")
    if computer == "scissors":
        print("computer", computer)
        print("player", player)
        print("You lose,sucker")
elif player == "scissors":
    if computer == "paper":
        print("computer", computer)
        print("player", player)
        print("You win")
    if computer == "rock":
        print("computer", computer)
        print("player", player)
        print("You lose,sucker")
