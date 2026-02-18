# snake-gun-water
#code of snake gun water game using python

j=0;
m=0;
print("welcome to snake,water,gun game!\n Enter snake water or gun as ur input")
for i in range(0,5):

    h=str(input("Enter Your Input for this game snake water gun game: "))
    import random
    s=["snake","water","gun"]
    a=random.choice(s)
    print(a)
    if h=="snake" and a=="gun":
        print("You LOSE")
        m+=1
        print(f'Your score is:{j} and computer score is:{m}')
        print(f'{4-i} chances left out of 5')
    elif h=="water" and a=="snake":
        print("You lose")
        m+=1
        print(f'Your score is:{j} and computer score is:{m}')
        print(f'{4 -i} chances left out of 5')
    elif h=="gun" and a=="snake":
        print("You win")
        j+=1
        print(f'Your score is:{j} and computer score is:{m}')
        print(f'{4- i} chances left out of 5')
    elif h=="gun" and a=="water":
        print("You lose")
        m+=1
        print(f'Your score is:{j} and computer score is:{m}')
        print(f'{4 - i} chances left out of 5')
    elif h=="snake" and a=="water":
        print("You win")
        j+=1
        print(f'Your score is:{j} and computer score is:{m}')
        print(f'{4 - i} chances left out of 5')
    elif h=="snake" and a=="snake":
        print("its a tie")
        print(f'Since its a tie there is no change in score so Your score is:{j} and computer score is:{m}')
        print(f'{4 - i} chances left out of 5')
    elif h=="water" and a=="water":
        print("its a tie")
        print(f'Since its a tie there is no change in score so Your score is:{j} and computer score is:{m}')
        print(f'{4 - i} chances left out of 5')
    elif h=="water" and a=="gun":
        print("u win")
        j+=1
        print(f'Your score is:{j} and computer score is:{m}')
        print(f'{4 - i} chances left out of 5')
    elif h=="gun" and a=="gun":
        print("you tie")
        print(f'Since its a tie there is no change in score so Your score is:{j} and computer score is:{m}')
        print(f'{4- i} chances left out of 5')
    else:
        print("improper i/p")
print(f"Your Score is: {j} and computer score is:{m}")
if m<j:
    print("You are the winner,Congratulations!!!")
elif m>j:
    print("you lose,BETTER LUCK NEXT TIME")
else:
    print("its a tie match")
