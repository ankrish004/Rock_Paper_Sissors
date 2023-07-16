# Rock_Paper_Sissors
rock paper and scissors game

rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇
import random

your = int(input(" enter 0 for rock , 1 for paper and 2 for scissor: "))

cpu = random.randint(0,2)


if  your >= 3 or your < 0:
  print("invalid ans")

else:
  image = [rock,paper,scissors]
  print(image[your-1])
  print(image[cpu-1])
  if your > cpu:
   print("you win")
  elif your == cpu:
   print("its a draw")
  elif your == 0 and cpu == 2:
    print("you win")
  elif your == 1 and cpu == 0:
    print("you win!")
  elif cpu == 0 and your == 2:
    print("you lose")
