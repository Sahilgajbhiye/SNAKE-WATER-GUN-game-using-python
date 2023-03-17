# SNAKE-WATER-GUN-game-using-python
SNAKE WATER GUN game

import random
print("THIS IS AN WATER SNAKE AND GUN GAME\n\n")
print("IF YOU WANT SNAKE TYPE s\nIF YOU WANT WATER TYPE w\nIF YOU WANT GUN TYPE g")
d=0
e=10
yourwincount = 0
computerwincount=0
while d<e:
    player1 = input("your turn :")
    player2 = ("s","w","g")
    c=random.choice(player2)
    if player1 == "s" and c == "s":
        print("you have chosen a SNAKE , player2 has also chosen SNAKE  \nso it is an TIE")
    if player1 == "s" and c == "w":
        print("you have chosen a SNAKE , player2 has also chosen WATER  \nso you have WON")
        yourwincount += 1
    if player1 == "s" and c == "g":
        print("you have chosen a SNAKE, player2 has also chosen GUN  \nyou have LOST")
        computerwincount+=1
    if player1 == "w" and c == "s":
        print("you have chosen a WATER , player2 has also chosen SNAKE  \nso you have WON")
        yourwincount += 1
    if player1 == "w" and c == "g":
        print("you have chosen a WATER , player2 has also chosen GUN  \nyou have WON")
        yourwincount += 1
    if player1 == "w" and c == "w":
        print("you have chosen a WATER , player2 has also chosen WATER  \nits an TIE")
    if player1 == "g" and c == "g":
        print("you have chosen a GUN , player2 has also chosen GUN  \nits an TIE")
    if player1 == "G" and c == "s":
        print("you have chosen a GUN , player2 has chosen SNAKE \nyou have WON")
        yourwincount += 1
    if player1 == "G" and c == "w":
        print("you have chosen a GUN , player2 has chosen WATER \nyou have LOST")
        computerwincount+=1
    if player1!= "w" or "s" or "g":
        print("you havent chose s, w, or g")
    d = d+1
if yourwincount>computerwincount:
    print(f"you have won by{yourwincount}")
else:
    print(f"you have lost by{computerwincount}")

    
