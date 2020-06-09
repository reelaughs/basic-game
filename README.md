# basic-game
A simple number guessing game featuring some very basic Python 

#same but with tiny difference. branch is for "what-if"/alternate code 

from random import randint
print("Let's see if you can guess the number in my head. The range is 1-100")
answer=randint(1,100)
guess=int(input("Guess a number\n"))
while answer != guess: 
    if answer < guess:
        print("Your guess is too high!")
    else:
        print("Your guess is too low!")
    guess= int(input("your guess? "))
print("Correct!")
