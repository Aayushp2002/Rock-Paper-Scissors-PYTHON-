# Rock-Paper-Scissors-PYTHON-
# One player Rock Paper Scissor game where you go against a computer

from random import randint

choices=["rock","paper","scissors"]
def main():
    computer=choices[randint(0,2)]

    print("Welcome to my game of rock, paper and scissors")
    question=input("Your choice (rock, paper, scissors): ").lower()
    print("Computer Chose: ",computer)

    if question==computer:
        print("It is a tie")
    elif question=="rock" and computer=="paper":
        print("Computer wins!")
    elif question=="rock" and computer=="scissors":
        print("Computer wins!")
    elif question=="paper" and computer=="rock":
        print("You win!")
    elif question=="paper" and computer=="scissors":
        print("Computer wins!")
    elif question=="scissors" and computer=="rock":
        print("Computer wins!")
    elif question=="scissors" and computer=="paper":
        print("You win!")
    else:
        print("Invalid input")

    main()
main()
