# basic-game
A simple number guessing game featuring the basics

#initial 

from random import randint
print("Let's see if you can guess the number in my head. The range is 1-100")
answer=randint(1,100)
guess=int(input("Guess a number"))
while answer != guess: 
    if answer > guess:
        print("Your guess is too low!")
    else:
        print("Your guess is too high")
    guess= int(input("And your guess is? "))
print("Correct!")
    
