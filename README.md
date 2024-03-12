# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not

ANSWER:-

#a) write the first letter of your name.
for row in range(6):
    for col in range(6):
        if col==0 or col==5 or(row==col and (col>0 and col<5)):
            print("*",end="")
        else:
            print(end=" ")
    print()
      
#b) print your name by using for loop.
name="Nandini"
for letters in name:
    print (letters)

#c) Check whether user name is palindrome or not.
def palindrome(word):
    x=word.replace(" ","")
    return x==x[::-1]

username = input("Enter your name:-")

if palindrome(username):
    print(f"{username} is a palindrome!")
else:
    print(f"{username} is not a palindrome.")

