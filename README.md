import random 

secret_num=random.randint(1,5)
chances=3
while chances >0:
    guess=int(input("Guess a num between 1-5:"))
              
    if guess==secret_num:
              print("You won")
              break 
    chances-=1
    print("Wrong guess")
    print("you chances:",chances)

    if chances==0:
        print("Game over")
        print("The num was:",secret_num)
