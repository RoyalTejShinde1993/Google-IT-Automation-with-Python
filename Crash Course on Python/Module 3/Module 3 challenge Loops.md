## 1. Fill in the blanks to print the numbers from 15 to 5, counting down by fives.
          
## Answers:
            number = 15 # Initialize the variable
            while number >= 5: # Complete the while loop condition
            print(number, end=" ")
            number -=5 # Increment the variable
            
            Output:15 10 5 

## 2.  Find and correct the error in the for loop below.  The loop should print every even number from 2 to 12.

## Answers:
          for number in range(2,13,2):
              print(number)

 Output: 2  4  6  8  10  12

 ## 3.  Fill in the blanks to complete the function “digits(n)” to count how many digits the given number has. For example: 25 has 2 digits and 144 has 3 digits. 
       Tip: you can count the digits of a number by dividing it by 10 once per digit until there are no digits left.

## Answers:
            def digits(n):
                count = 0
              if n == 0:
                 count += 1
              while n > 0: # Complete the while loop condition
                           # Complete the body of the while loop. This should include 
                           # performing a calculation and incrementing a variable in the
                           # appropriate order.  
                n //= 10
                count += 1
              return count
    
            print(digits(25))   # Should print 2
            print(digits(144))  # Should print 3
            print(digits(1000)) # Should print 4
            print(digits(0))    # Should print 1
            
## 4. Fill in the blanks to complete the “rows_asterisks” function. This function should print rows of asterisks (*), where the number of rows is equal to the “rows” variable. The number of asterisks per row should correspond to the row number (row 1 should have 1 asterisk, row 2 should have 2 asterisks, etc.). Complete the code so that “row_asterisks(5)” will print:

## *
## **
## ***
## ****
## *****
## Answers:
            def rows_asterisks(rows):
            # Complete the outer loop range to control the number of rows
            for x in range(1,rows+1): 
                  # Complete the inner loop range to control the number of 
                  # asterisks per row
            for y in range(x): 
                     # Prints one asterisk and one space
                print("*", end=" ")
            # An empty print() function inserts a line break at the 
            # end of the row 
            print()


            rows_asterisks(5)

## 5.  Fill in the blanks to complete the “counter” function. This function should count down from the “start” to “stop” variables when “start” is bigger than “stop”. Otherwise, it should count up from “start” to “stop”. Complete the code so that a function call like “counter(3, 1)” will return “Counting down: 3, 2, 1” and “counter(2, 5)” will return “Counting up: 2, 3, 4, 5”.

## Answers:
           def counter(start, stop):
               if start > stop:
                      return_string = "Counting down: "
                while start>=stop: # Complete the while loop
                      return_string += str(start) # Add the numbers to the "return_string"
              if start > stop:
                      return_string += ","
                 start -= 1 # Increment the appropriate variable
              else:
                      return_string = "Counting up: "
                while start <= stop: # Complete the while loop
                      return_string += str(start) # Add the numbers to the "return_string"
                if start < stop:
                      return_string += ","
                  start += 1 # Increment the appropriate variable
                return return_string

              print(counter(1, 10)) # Should be "Counting up: 1,2,3,4,5,6,7,8,9,10"
              print(counter(2, 1)) # Should be "Counting down: 2,1"
              print(counter(5, 5)) # Should be "Counting up: 5"

## 6. Fill in the blanks to complete the “odd_numbers” function. This function should return a space-separated string of all odd positive numbers, up to and including the “maximum” variable that's passed into the function. Complete the for loop so that a function call like “odd_numbers(6)” will return the numbers “1 3 5”.


## Answers:
            def odd_numbers(maximum):
    
                return_string = "" # Initializes variable as a string

            # Complete the for loop with a range that includes all 
            # odd numbers up to and including the "maximum" value.
            for num in range(1, maximum + 1, 2): 

                # Complete the body of the loop by appending the odd number
                # followed by a space to the "return_string" variable.
           return_string += str(num) + " "  

           # This .strip command will remove the final " " space 
           # at the end of the "return_string".
          return return_string.strip()



          print(odd_numbers(6))  # Should be 1 3 5
          print(odd_numbers(10)) # Should be 1 3 5 7 9
          print(odd_numbers(1))  # Should be 1
          print(odd_numbers(3))  # Should be 1 3
          print(odd_numbers(0))  # No numbers displayed

## 7. What happens when the Python interpreter executes a loop where a variable used inside the loop is not initialized?

## Answers:  Will produce a NameError stating the variable is not defined

## 8. How many numbers will this loop print?  Your answer should be only one number. 
      
      for sum in range(5):
          sum += sum
          print(sum)
          
## Answers: 5

## 9. What is the initial value of  the “outer_loop” variable on the first iteration of the nested "inner_loop"? Your answer should be only one number. 

       for outer_loop in range(2, 6+1):
           for inner_loop in range(outer_loop):
                if inner_loop % 2 == 0:
                    print(inner_loop)

## Answers: 2

## 10. The following code causes an infinite loop. Can you figure out what’s incorrect and how to fix it?

          def count_to_ten():
              x = 1
            while x <= 10:
              print(x)
            x = 1

          count_to_ten()
## Answers:  1 2 3 4 5 6 7 8  9 10
