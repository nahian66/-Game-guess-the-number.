# game guess the number.

a = 31
i = 0
for i in range(1, 10):

    n = int(input("Guess the number= "))
    
    if i < 9 or n == 20:
       if n < a:
            print("You guessed the wrong number.")
            print("Please increase your number.")
            print("Your chance remaining: ", 9-i)

       elif n > a:
            print("You guessed the wrong number.")
            print("Please decrease your number.")
            print("Your chance remaining: ", 9-i)

       else:
            print("Congratulations!!!")
            print("You guessed the right number in ", i , "chances.")
            break
    else:
          print("You guessed the wrong number.")
          print("Your chance remaining: ", 9-i)
          print("Game Over!!!!!!")
