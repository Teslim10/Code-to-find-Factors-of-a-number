# Code-to-find-Factors-of-a-number
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
