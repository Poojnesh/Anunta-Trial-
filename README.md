import random
import math
# Who is even who is odd? due:2/14
#Poojaa and Kwadwo

#comment:These are fixed values 
choice_one= "odd"
choice_two= "even"

# When each side wins
computer_wins = choice_one
user_wins = choice_two


#input
user_choice = int(input("Enter number between 1 to 5: "))
#Random computer choice
computer_choice = random.randint(1,5)
total_choice = user_choice+computer_choice
# remainder to figure out even and odd
remainder = total_choice%2
if(remainder>0):
    result= choice_one
else:
    result= choice_two

#output    
print("This is user choice: ",user_choice)
print("This is computer choice: ", computer_choice)
print("The final sum of user and computer:", total_choice)
print("The number is: ", result)
if(result==choice_one):
    print("computer wins!")
else:
    print("User wins!")
    


    
