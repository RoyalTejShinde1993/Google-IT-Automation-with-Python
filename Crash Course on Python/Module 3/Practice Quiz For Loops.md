## 1  In Python, what do while loops do?

## Answers:while loops tell the computer to repeatedly execute a set of instructions while a condition is true.

## 2 Which techniques can prevent an infinite while loop? Select all that apply.

## Answers:
          Change the value of a variable used in the while condition

## 3 The following code contains an infinite loop, meaning tthe Python interpreter does not know when to exit the loop once the task is complete. To solve the problem, you will need to:

Find the error in the code

Fix the while loop so there is an exit condition

Hint: Try running your function with the number 0 as the input and observe the result.

Note that Coursera’s code blocks will time out after 5 seconds of running an infinite loop. If you get this timeout error message, it means the infinite loop has not been fixed.
def is_power_of_two(number):

  if number <= 0:
    return False
    
  while number % 2 == 0:
    number = number // 2  # Use integer division to prevent float conversion
  
  return number == 1

Calls to the function
print(is_power_of_two(0))  # Should be False
print(is_power_of_two(1))  # Should be True
print(is_power_of_two(8))  # Should be True
print(is_power_of_two(9))  # Should be False

## 4 Write a function that takes an argument n and returns the sum of integers from 1 to n. For example, if n=5, your function should add up 1+2+3+4+5 and return 15. If n is less than 1, just return 0. Use a while loop to calculate this sum. 
 def sum_of_integers(n):
   if n < 1:
     return 0

   i = 1
   sum = 0  # Initialize sum to 0
    while i <= n:  # Loop until i reaches n
       sum = sum + i
       i = i + 1  # Increment i

  return sum

print(sum_of_integers(3))  # should print 6
print(sum_of_integers(4))  # should print 10
print(sum_of_integers(5))  # should print 15
### 5 Fill in the blanks to complete the function, which should output a multiplication table. The function accepts a variable “number” through its parameters. This “number” variable should be multiplied by the numbers 1 through 5, and printed in a format similar to “1x6=6” (“number” x “multiplier” = “result”). The code should also limit the “result” to not exceed 25. To satisfy these conditions, you will need to:

 Initialize the “multiplier" variable with the starting value

 Complete the while loop condition

 Add an exit point for the loop

 Increment the “multiplier" variable inside the while loop

def multiplication_table(number):
    # Initialize the appropriate variable
    ___ = ___


    # Complete the while loop condition.
    while ___:
        result = number * multiplier 
        if  result > 25:
            # Enter the action to take if the result > 25
            ___
        print(str(number) + "x" + str(multiplier) + "=" + str(result))
        
        # Increment the appropriate variable
        ___ += 1


multiplication_table(3) 
 Should print: 
 3x1=3 
 3x2=6 
 3x3=9 
 3x4=12 
 3x5=15


multiplication_table(5) 
Should print: 
 5x1=5
 5x2=10
 5x3=15
 5x4=20
 5x5=25

multiplication_table(8) 
 Should print:
 8x1=8
 8x2=16
 8x3=24

### Answers ###
def multiplication_table(number):
    # Initialize the appropriate variable
    multiplier = 1  # Start from 1

    # Complete the while loop condition.
    while multiplier <= 5:  # Loop runs from 1 to 5
        result = number * multiplier
        if result > 25:
            # Enter the action to take if the result > 25
            break  # Stop the loop if result exceeds 25
        print(str(number) + "x" + str(multiplier) + "=" + str(result))
        
        # Increment the appropriate variable
        multiplier += 1  # Increment the multiplier

### Answers ###
3x1=3
3x2=6
3x3=9
3x4=12
3x5=15
5x1=5
5x2=10
5x3=15
5x4=20
5x5=25
8x1=8
8x2=16
8x3=24
