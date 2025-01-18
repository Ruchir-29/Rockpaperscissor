# Rockpaperscissor
#if you like ths code make  sure to comment.

"""
Workflow for the game
1-Input from user(Rock,Paper,Scissor)
2-Computer choice(Rock,Paper,Scissor)
computer will choose randomly not conditionally
3-print result

Cases
1-User chooses Rock
rock-rock = tie
rock-paper = paper wins
rock-scissor = rock wins

2-user chooses paper
paper-paper = tie
paper-scissor = scissor wins
paper-rock = rock wins

3-user chooses scissor
scissor-scissor = tie
scissor-paper = scissor wins
scissor-rock = rock wins
"""

import random
option_list=["Rock","Paper","Scissor"]

print("Rock,paper,scissor")

user_choice = input("Enter Your choice: ")
comp_choice =  random.choice(option_list)

print(f"Users choice = {user_choice}, Computer Choice = {comp_choice}")
if user_choice == comp_choice:
    print("Match Tie")

elif user_choice == "Rock":
    if comp_choice == "Paper":
        print("Paper covers Rock , Computer Wins")
    else:
        print("Rock smashes Scissor , User Wins")

elif user_choice == "Paper":
    if comp_choice == "Scissor":
        print("Scissor cuts Paper , Computer Wins")
    else:
        print("Paper Covers Rock , User Wins")

elif user_choice == "Scissor":
    if comp_choice == "Rock":
        print("Rock smashes Scissor , Computer Wins")
    else:
        print("Scissor cuts Paper,User Wins")

else:
    print("Invalid Input")


#thanks for using the program, appreciate if ypu would comment in my GitHub
