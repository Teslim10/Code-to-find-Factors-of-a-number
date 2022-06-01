# Code-to-find-Factors-of-a-number
'''The factors of a number are those lesser (and equal) positive integers that can easily divide a number without giving remainders.
For example, the factors of 6 are 1, 2, 3 and 6.
The factors of 15 are 1, 3, 5 and 15.
Write a program that finds all the factors of a particular given number, N.
The program first takes an input from the user, and raises an exception, if the input is not a positive integer. If the exception is passed, it prints the factors of N.
If for instance, N is given as -8.2, the program raises an exception saying "Wrong input!"
If N is 36, it prints:
➖➖➖➖➖➖➖➖➖➖➖
The factors of 36 are 1, 2, 3, 4, 6, 9, 12, 18 and 36.
➖➖➖➖➖➖➖➖➖➖➖
Include comments in your code.'''
try:
    def print_factors(number): #defines the function to print factors of a number
        print("The factors of",number,"are:")
        x = int(number)
        if isinstance(x, int) == True and x > 0: # checks if inputted number is a positive integer
            for i in range(1, x+1):
                if x % i == 0: #tests if a number is a factor of the user inputted number
                    print(i)
                else:
                    pass
        else:
            print("Invalid input")
except ValueError:
    print("invalid input")
number = input("Enter your number:\n") #asks for user input
print_factors(number)
