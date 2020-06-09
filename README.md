# basic-game
A simple number guessing game featuring the basics

  #My initial answer. Game might go something like this
... #1. Instructions
... #2. Pick a number between 1-100.
... #3. Guess midpoint. If correct, game ends.
... #4. If guess is higher, then guess higher than previous midpoint
... #5 If guess is lower, than guess lower than previous midpoint
... #6. If guess is correct, game ends. If not, start from Step 3 again with the new reduced interval.

#better Instructions, turning into code 
... #1. Pick a number to be your answer
... #2. Player has a guess- guess
... #3. Check if answer and guess are the same- CONGRATS! if yes
... #4. #Is answer less than guess- tell them to guess higher
... #5. #If answer is greater than guess- tell them to guess lower
... #6. #Go back to step 3

  

from random import randint
print("Let's see if you can guess the number in my head. The range is 1-100")
answer=randint(1,100)
guess=int(input("Guess a number\n"))
while answer != guess: 
    if answer > guess:
        print("Your guess is too low!")
    else:
        print("Your guess is too high")
    guess= int(input("your guess? "))
print("Correct!")
    
   
    
